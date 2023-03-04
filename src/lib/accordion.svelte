<script lang="ts">
	import { slide } from 'svelte/transition';
	export let question: string;
	export let answer: string;
	let isOpen = false;
	const toggle = () => (isOpen = !isOpen);
</script>

<div>
	<button
		on:click={toggle}
		aria-expanded={isOpen}
		class="flex w-full items-center gap-1 py-2 hover:drop-shadow-md"
	>
		<svg
			style="tran"
			width="20"
			height="20"
			fill="none"
			stroke-linecap="round"
			stroke-linejoin="round"
			stroke-width="2"
			viewBox="0 0 24 24"
			stroke="currentColor"><path d="M9 5l7 7-7 7" /></svg
		>
		<p class="text-left max-w-[90%]">{question}</p>
	</button>
	{#if isOpen}
		<p transition:slide={{ duration: 300 }} class="ml-6 my-3 max-w-[50%]">{answer}</p>
	{/if}
</div>

<style lang="postcss">
	svg {
		transition: transform 0.2s ease-in;
	}

	[aria-expanded='true'] svg {
		transform: rotate(0.25turn);
	}
</style>
