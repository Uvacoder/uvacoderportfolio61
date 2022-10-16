<script>
  import '../app.css'
  import '../prism.css'
  import 'focus-visible'
  import MoonIcon from 'heroicons-svelte/solid/MoonIcon.svelte'
  import SunIcon from 'heroicons-svelte/solid/SunIcon.svelte'
  import { browser } from '$app/env'
  import { name } from '$lib/info'
  import NavLink from '$lib/components/NavLink.svelte'

  let prefersLight = browser ? Boolean(JSON.parse(localStorage.getItem('prefersLight'))) : false
</script>

<div class="flex flex-col min-h-screen">
  <div class="max-w-4xl mx-auto flex flex-col flex-grow w-full">
    <div class="flex h-16 px-4 py-2 justify-between items-center">
      <nav class="flex items-center space-x-4 sm:space-x-8">
        <NavLink href="/">uvacoder</NavLink>
        <NavLink href="/projects">projects</NavLink>
        <NavLink href="/blog">blog</NavLink>
      </nav>
      {#if browser}
        <button
          type="button"
          role="switch"
          aria-label="Toggle Dark Mode"
          aria-checked={!prefersLight}
          class="h-4 w-4 sm:h-8 sm:w-8 sm:p-1"
          on:click={() => {
            prefersLight = !prefersLight
            localStorage.setItem('prefersLight', prefersLight.toString())

            if (prefersLight) {
              document.querySelector('html').classList.remove('dark')
            } else {
              document.querySelector('html').classList.add('dark')
            }
          }}
        >
          {#if prefersLight}
            <MoonIcon class="text-slate-500" />
          {:else}
            <SunIcon class="text-slate-400" />
          {/if}
        </button>
      {/if}
    </div>
    <main
      class="mt-4 flex flex-col w-full flex-grow py-4 px-4 prose prose-slate prose-sm sm:prose sm:prose-slate sm:prose-lg sm:max-w-none dark:prose-invert"
    >
      <slot />
    </main>
  </div>
</div>
