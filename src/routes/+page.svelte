<script lang="ts">
	import GuildedLogo from '../assets/Guilded_White.svg';
</script>

<main class="flex flex-col m-20">
	<h1 class="h1">BetterGuilded</h1>
	<p>
		Welcome to BetterGuilded, the community-driven project to improve the Guilded experience for
		everyone.
		<br />
		BetterGuilded is a third-party software that allows you to inject plugins and themes into Guilded
		to enhance your experience.
	</p>
	<div class="mt-5">
		<div class="flex items-center space-x-4">
			<a href="https://github.com/BetterGuildedgg" target="_blank">
				<button class="rounded bg-primary-500 p-3 flex justify-center items-center w-32">
					<span class="text-white"> GitHub </span>
				</button>
			</a>
			<button class="rounded bg-primary-500 p-2 flex justify-center items-center w-32">
				<img src={GuildedLogo} class="size-8" alt="Guilded" />
				<span class="text-white">Guilded</span>
			</button>
		</div>
	</div>
	<div class="mt-20">
		<h1 class="h2">What does BetterGuilded offer?</h1>
		<p>
			BetterGuilded offers community-crafted plugins and themes to enhance your Guilded experience.
			<br />
			You can find a list of all available plugins and themes on the <a href="/plugins">Plugins</a>
			and <a href="/themes">Themes</a> page.
		</p>
	</div>
	<div class="mt-20">
		<h1 class="h2">BetterGuilded for developers</h1>
		<p>
			Currently BetterGuilded is in early development and we are looking for contributors to help,
			there is no addons/plugins/themes API or system quite yet.
		</p>
	</div>
</main>
