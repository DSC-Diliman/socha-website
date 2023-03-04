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

<nav class="sticky top-0 flex w-full justify-center gap-2 bg-white">
	{#each links as { id, name }}
		<div>
			<a href="/#{id}">{name}</a>
		</div>
	{/each}
</nav>

<style lang="postcss"></style>
