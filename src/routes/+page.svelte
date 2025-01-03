<script lang="ts">
import GuildedLogo from '$lib/assets/GuildedLogo.svg';
import { contributors } from '$lib/contributors';
import { Avatar } from '@skeletonlabs/skeleton';
</script>

<div class="container m-20">
<div class="space-y-5">
		<h1 class="h1 max-w-3xl">BetterGuilded.</h1>
		<p class="blockquote font-semibold">
			A third-party software that allows you to inject plugins and themes into Guilded to enhance your experience.
		</p>
		<div class="flex gap-4">
			<button class="btn variant-filled-primary p-3 px-12 rounded-md">
				GitHub
			</button>
			<button class="btn variant-filled-primary p-3 px-6 rounded-md flex items-center">
				<img src={GuildedLogo} alt="" class="w-8 h-8 mr-2" />
				Guilded
			</button>
		</div>
	</div>
</div>
<div class="py-20">
	<div class="justify-center items-center flex">
		<div class="alert variant-glass-primary flex gap-1 p-6 px-20">
			<a href="https://github.com/BetterGuildedgg"> @BetterGuildedgg </a> is looking for contributors
		</div>
	</div>
</div>
<div class="container m-20">
	<div class="space-y-5">
		<h1 class="h1">100% Free and<br>Open Source.</h1>
		<p class="lg max-w-56">
			BetterGuilded is completely free and open source and can be found on <a href="https://github.com/BetterGuildedgg" class="text-[#da5597] duration-300 hover:text-[#fb62ae]">GitHub</a>
		</p>
	</div>
</div>
<div id="contributors" class="w-full h-1 bg-white/15"></div>
<br>
<div class="h-screen flex flex-col justify-center items-center text-center">
	<h1 class="h1">
		Awesome people
	</h1>
	<br>
	<p class="lg max-w-56 mb-24">
		The awesome people that help make the BetterGuilded project possible.
	</p>
	<ul class="flex flex-col">
		{#each contributors as contributor}
			<li class="flex flex-row">
				<div class="relative inline-block">
					<Avatar src={contributor.avatar_url} />
				</div>
				<div class="flex flex-col">
					<p class="badge variant-filled h-5">{contributor.roles.join(', ')}</p>
					<a href={contributor.url} class="p-2">{contributor.username}</a>
					{#if contributors.length > 1}
						<br />
					{/if}
				</div>
			</li>
		{/each}
	</ul>
</div>
