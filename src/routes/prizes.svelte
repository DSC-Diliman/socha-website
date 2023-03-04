<script lang="ts">
	interface Award {
		prize: string;
		award: string;
		color: string;
	}

	const awards: Award[] = [
		{
			prize: 'PHP 10,000',
			award: '1ST RUNNER UP',
			color: 'bg-gradient-to-r from-[#70706F] to-[#BEC0C2]'
		},
		{
			prize: 'PHP 5,000',
			award: '2ND RUNNER UP',
			color: 'bg-gradient-to-r from-[#804A00] to-[#B08D57]'
		},
		{
			prize: 'PHP 3,000',
			award: 'BEST INNOVATION PROPOSAL',
			color: 'bg-gradient-to-r from-purple-500 to-orange-500'
		}
	];
</script>

<section class="py-20 px-8" id="prizes">
	<h1 class="mb-16 text-center text-6xl font-bold">Prizes</h1>
	<div class="mb-10 flex flex-col items-center">
		<h2
			class="mb-2 bg-gradient-to-r from-[#B78628] to-[#FCC201] bg-clip-text text-5xl font-bold text-transparent"
		>
			PHP 20,000
		</h2>
		<p class="text-2xl font-extrabold">GRAND WINNER</p>
	</div>
	<div class="flex flex-col items-center justify-center gap-10 lg:flex-row">
		{#each awards as { prize, award, color }}
			<div class="flex w-56 flex-col items-center">
				<h2 class="{color} mb-1 bg-clip-text text-4xl font-bold text-transparent">{prize}</h2>
				<p class="font-bold">{award}</p>
			</div>
		{/each}
	</div>
	<p class="my-5 text-center text-5xl">+</p>
	<div class="text-center font-bold">
		<p>EXCLUSIVE EVENT FROM ACCENTURE</p>
		<p>CERTIFICATE OF PARTICIPATION</p>
	</div>
</section>

<style lang="postcss"></style>
