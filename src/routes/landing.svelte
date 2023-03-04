<script>
	let linkData = [
		{
			link: 'bit.ly/SolCha23_RegForm',
			text: 'Register now!'
		},
		{
			link: 'https://www.facebook.com/DilimanSoCha',
			text: 'Visit our Facebook page!'
		}
	];
</script>

<section class="flex flex-col gap-10 px-8 py-16" id="landing">
	<h1 class="text-center text-5xl font-bold italic sm:text-7xl">
		<p
			class="bg-gradient-to-r from-purple-500 to-orange-500 bg-clip-text px-3 font-extrabold text-transparent"
		>
			Diliman Solutions
		</p>
		<p
			class="bg-gradient-to-r from-purple-500 to-orange-500 bg-clip-text px-3 pb-1 font-extrabold text-transparent sm:pb-3"
		>
			Challenge 2023
		</p>
	</h1>
	<p class="mx-auto sm:max-w-[80%] lg:max-w-[60%] xl:max-w-[40%]">
		The Diliman Solutions Challenge is the flagship event of the Google Developer Student Clubs UP
		Diliman. This event seeks to call all students to ideate, innovate, and integrate relevant and
		effective solutions to pressing issues in local communities and the country, through the use of
		Google technology. Experience Google technology firsthand and pave the way for the youth to
		build a better tomorrow.
	</p>
	<div class="mx-auto flex gap-5">
		{#each linkData as { link, text }}
			<a
				href={link}
				class="rounded-md bg-[#7b1113] px-4 py-1 text-lg text-white transition-all hover:scale-110"
				>{text}</a
			>
		{/each}
	</div>
</section>

<style lang="postcss"></style>
