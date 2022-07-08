<script>
  import ButtonLink from '$lib/components/ButtonLink.svelte'
  import PostPreview from '$lib/components/PostPreview.svelte'
  import { name } from '$lib/info.js'

  export let recentPosts
</script>

<svelte:head>
  <title>{name}</title>
</svelte:head>

<div class="container px-6 py-16 mx-auto text-center">
  <div class="max-w-lg mx-auto">
    <h1 class="mb-3 text-3xl font-bold tracking-tight text-black dark:text-white md:text-5xl">
      Akash
      <span
        class="relative ml-2 inline-block before:absolute before:-inset-1 before:block before:-skew-y-3 before:bg-gradient-to-r from-blue-500 to-teal-500 dark:from-violet-500 dark:to-pink-500"
        ><span class="relative skew-y-3 text-white">@ak4zh</span></span
      >
      Agarwal
    </h1>

    <div class="mt-8 space-y-2">
      <p class="mt-6 text-gray-500 dark:text-gray-300">
        <span class="mx-2">A self-taught full stack developer</span>
      </p>

      <p class="mt-6 text-gray-700 dark:text-gray-200 font-light">
        <span class="mx-2">Learning by doing is the only way I know how to learn.</span>
      </p>
    </div>
  </div>

  <!-- recent posts -->
  <h2 class="flex items-baseline gap-4 !mb-2">
    Recent Posts
    <ButtonLink href="/posts" size="small" raised={false} class="opacity-60">View All</ButtonLink>
  </h2>
  <div class="grid gap-4 grid-cols-1 sm:grid-cols-2">
    {#each recentPosts as post}
      <div class="flex p-4 border border-slate-300 dark:border-slate-700 rounded-lg">
        <PostPreview {post} small />
      </div>
    {/each}
  </div>
</div>
