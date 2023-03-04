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
			id: 'sponsors',
			name: 'Sponsors'
		},
		{
			id: 'faq',
			name: 'FAQ'
		}
	];
</script>

<nav>
	{#each links as { id, name }}
		<a href="/#{id}">{name}</a>
	{/each}
</nav>

<style>
	nav {
		position: sticky;
		top: 0px;
		background-color: white;
	}
</style>
