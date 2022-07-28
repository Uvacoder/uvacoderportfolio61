<script>
	import Project from '$lib/components/Project.svelte'
	import ButtonLink from '$lib/components/ButtonLink.svelte'
</script>

<svelte:head>

<title>ak4zh | Projects</title>
</svelte:head>

<div class="space-y-8">
	<Project
			title="bummer"
			img="/bummer.png"
			web="https://bummer.me"
		>
		One way to make your career regrets “less fearsome” is by talking to people about them. Bummer let’s you create a résumé of your failures and share it in the open.
	</Project>
	<Project
			title="Stooge"
			img="/stooge.png"
			web="https://stooge.me"
		>
		We all love comics. Comics are an amazing tool for storytelling. But I cannot even draw a perfect circle. So I have created stooge, a comic creator app to help educators and storytellers make comics without the need to draw.
	</Project>
	<Project
		title="ConfluxBot"
		img="/confluxbot.svg"
		web="https://confluxbot.com"
	>
	ConfluxBot merges all your social media accounts at one place and let them flow together. In the ConfluxBot dashboard you can connect many of your social media accounts like Telegram, Discord, Reddit, Personal Blogs etc.
Then you can create connections between these accounts to make fully synced and completely automated posts across each connected platform.
	</Project>
	<Project
		title="Statera"
		web="http://statera.in"
        img="/statera.png"
		github="https://github.com/ak4zh/statera"
	>
	An open source web app for all your accounting needs.
Statera is a small fun project I created while I was playing with SvelteKit (an application framework powered by svelte)

_Statera is just a fun project and not production ready. You can play around to get inspired or check the github repo to learn how it's built._
</Project>
<Project title="Cuddy" img="/cuddy.png" web="https://cuddy.me">
A free web app to make beautiful landing pages in minutes.</Project>
<Project
    	title="MijnBedrijfsWagenLease"
        img="/mijnbedrijfswagenlease.png"
    	web="https://mijnbedrijfswagenlease.nl">
A website to search for vehicles available for lease.
Pardon if the texts look alien to you, I built this website for a netherlands based business hence the website is in dutch language.

### Tech Stack
- #### Frontend
  - SvelteKit (javascript framework)
  - TailwindCSS (asthetics)
- #### Backend
  - Supabase (for database and auth)
  - Cloudflare Pages (hosting)
  
</Project>
    <Project
    	title="WAFAcademy"
        img="/wafacademy.png"
    	web="https://wafa.academy/catalogue/"
    	>
    An e-commerce website for a german company.
    </Project>
    <div class="flex justify-center sm:justify-end pb-8">
    		<ButtonLink href="https://github.com/ak4zh" rel="external">
    		Check out the rest on GitHub
    		</ButtonLink>
    </div>
</div>
