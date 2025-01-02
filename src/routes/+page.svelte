<script>
	import Banner from '../assets/images/BetterGuilded.png';
	import { MessageSquareMore } from 'lucide-svelte';
</script>

<main class="h-screen bg-[#14151b]">
	<div class="flex flex-col justify-center text-center items-center pt-60">
		<h1 class="h1">The Guilded Enhancement Project</h1>
		<p class="text-slate-500 mt-2 font-bold">
			BetterGuilded extends the functionality of Guilded by enhancing it with new features and
			themes.
		</p>
		<div class="flex gap-6 mt-8">
			<a href="https://github.com/BetterGuildedgg" target="_blank">
				<button class="btn bg-[#2f5b9d] max-w-3xl px-20 py-5 rounded-md flex-1"> GitHub </button>
			</a>
			<a href="https://guilded.gg/BetterGuilded" target="_blank">
				<button
					class="btn bg-transparent border border-slate-800 max-w-3xl px-20 py-5 rounded-md flex-1 text-slate-400"
				>
					<MessageSquareMore class="mr-3" />
					Community
				</button>
			</a>
		</div>
		<div class="mt-20">
			<img src={Banner} alt="BetterGuilded" class="aspect-auto" />
		</div>
	</div>
</main>
