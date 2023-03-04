<script>
	let links = [
		{
			id: 'landing',
			name: 'Top'
		},
		{
			id: 'description',
			name: 'Description'
		},
		{
			id: 'timeline',
			name: 'Timeline'
		},
		{
			id: 'rules',
			name: 'Rules'
		},
		{
			id: 'prizes',
			name: 'Prizes'
		},
		{
			id: 'speakers',
			name: 'Speakers'
		},
		{
			id: 'mentors',
			name: 'Mentors'
		},
		{
			id: 'credits',
			name: 'Credits'
		},
		{
			id: 'faq',
			name: 'FAQ'
		}
	];
</script>

<nav>
	{#each links as { id, name }}
		<div>
			<a href="/#{id}">{name}</a>
		</div>
	{/each}
</nav>

<style>
	nav {
		position: sticky;
		top: 0px;
		background-color: white;
		display: flex;
		width: 100%;
		justify-content: center;
		gap: 2em;
	}
</style>
