<script lang="ts">
	import { AppBar } from '@skeletonlabs/skeleton';
	import '../app.css';
</script>

<AppBar background="transparent">
	<svelte:fragment slot="lead"><a href="/"> BetterGuilded</a></svelte:fragment>
	<svelte:fragment slot="trail">
		<div class="flex items-center space-x-4">
			<a href="/contributors"> Contributors </a>
			<a href="https://guilded.gg/BetterGuilded"> Guilded </a>
			<a href="/contributors"> GitHub </a>
		</div>
	</svelte:fragment>
</AppBar>

<slot />
