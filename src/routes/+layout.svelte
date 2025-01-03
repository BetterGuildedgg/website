<script lang="ts">
	import '../app.postcss';
	import GuildedLogo from "$lib/assets/GuildedLogo.svg"
	import { AppBar } from '@skeletonlabs/skeleton';
	// Highlight JS
	import hljs from 'highlight.js/lib/core';
	import 'highlight.js/styles/github-dark.css';
	import { storeHighlightJs } from '@skeletonlabs/skeleton';
	import xml from 'highlight.js/lib/languages/xml'; // for HTML
	import css from 'highlight.js/lib/languages/css';
	import javascript from 'highlight.js/lib/languages/javascript';
	import typescript from 'highlight.js/lib/languages/typescript';

	hljs.registerLanguage('xml', xml); // for HTML
	hljs.registerLanguage('css', css);
	hljs.registerLanguage('javascript', javascript);
	hljs.registerLanguage('typescript', typescript);
	storeHighlightJs.set(hljs);
</script>


<AppBar background="transparent">
	<svelte:fragment slot="lead">
		<img src={GuildedLogo} alt="" class="size-16">
	</svelte:fragment>
	<a href="/">
		BetterGuilded
	</a>
	<svelte:fragment slot="trail">
		<a href="#contributors">Contributors</a>
		<a href="https://github.com/BetterGuildedgg/" target="_blank">GitHub</a>
		<a href="https://guilded.gg/BetterGuilded/" target="_blank">Guilded</a>
	</svelte:fragment>
</AppBar>


<slot />
