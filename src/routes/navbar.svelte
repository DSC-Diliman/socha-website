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

<nav
	class="sticky top-0 grid w-full grid-cols-3 grid-rows-3 justify-items-center gap-3 bg-white py-3 drop-shadow-md sm:flex sm:justify-center"
>
	{#each links as { id, name }}
		<div>
			<a href="/#{id}" class="rounded-md py-1 px-3 hover:bg-black hover:text-white">{name}</a>
		</div>
	{/each}
</nav>

<style lang="postcss"></style>
