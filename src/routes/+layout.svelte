<script lang="ts">
	import { AppBar } from '@skeletonlabs/skeleton';
	import '../app.css';
</script>

<AppBar background="bg-[#0c0d10] p-12">
	<svelte:fragment slot="lead"
		><a href="/" class="text-2xl">
			<span class="text-[#2f5b9d]">Better</span>Guilded</a
		></svelte:fragment
	>
	<svelte:fragment slot="trail">
		<div class="flex items-center space-x-4">
			<a href="/contributors"> Contributors </a>
			<a href="https://guilded.gg/BetterGuilded"> Guilded </a>
			<a href="https://github.com/BetterGuildedgg"> GitHub </a>
		</div>
	</svelte:fragment>
</AppBar>

<slot />
