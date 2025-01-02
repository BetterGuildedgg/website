<script lang="ts">
	import { Avatar } from '@skeletonlabs/skeleton';

	const contributors = [
		{
			username: 'Myferr',
			roles: ['Maintainer', 'Developer'],
			avatar_url: 'https://github.com/myferr.png',
			url: 'https://github.com/myferr'
		},
		{
			username: 'WeebTheDev',
			roles: ['Maintainer', 'Developer'],
			avatar_url: 'https://github.com/weebthedev.png',
			url: 'https://github.com/weebthedev'
		}
	];
</script>

<main class="flex flex-col m-20">
	<h1 class="h1">Contributors to our project!</h1>
	<p class="p">Here are the awesome people who have contributed to our projects</p>
	<br />
	<br />
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
</main>
