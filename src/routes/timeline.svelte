<script lang="ts">
	interface Event {
		duration: string;
		event: string;
		description: string;
		done: boolean;
		current: boolean;
	}

	let events: Event[] = [
		{
			duration: 'February 18 – March 5',
			event: 'REGISTRATION PERIOD',
			description:
				'Registration period will be open for over two weeks. Participants may register here.',
			done: true,
			current: false
		},
		{
			duration: 'February 20 – March 4',
			event: 'INTERACT: NETWORKING AVENUES',
			description: 'Meet and network with other participants through the event Discord channel.',
			done: true,
			current: false
		},
		{
			duration: 'March 4 – 5',
			event: 'IDEATE: 48-HOUR IDEATHON CHALLENGE',
			description:
				'A 48-hour intensive brainstorming session to come up with an innovation proposal along with activities to help the ideation process.',
			done: false,
			current: true
		},
		{
			duration: 'March 11 – 19',
			event: 'INNOVATE: PROTOTYPING PERIOD & MENTORSHIP SESSIONS',
			description:
				"This is the beginning of the team's prototype creation. The mentorship sessions are designed to guide teams in creating a successful prototype of their idea and preparing for a live pitch and an AVP. Teams receive feedback and consultations from mentors to refine their proposals and increase their chances of success for their final submissions.",
			done: false,
			current: false
		},
		{
			duration: 'March 25',
			event: 'IMPLEMENT: LIVE PITCHING DEMO DAY',
			description:
				'A 48-hour intensive brainstorming session to come up with an innovation proposal along with activities to help the ideation process.',
			done: false,
			current: false
		},
		{
			duration: 'March 25',
			event: 'AWARDING CEREMONY',
			description:
				'On the same day of the live pitching, winners will be announced. Do you have what it takes to reach the top?',
			done: false,
			current: false
		}
	];
</script>

<section class="py-20 px-8" id="timeline">
	<h1 class="mb-10 text-center text-6xl font-bold">Timeline</h1>
	<div class="flex flex-col items-center gap-10 px-10">
		{#each events as { duration, event, description, done, current }}
			<div
				class="relative box-content w-80 rounded-xl border border-solid border-[#7b1113] bg-white py-5 px-10 {done &&
					'opacity-50'}"
			>
				<p class="mb-1 font-bold">{duration}</p>
				<h2 class="mb-4">{event}</h2>
				<p>{description}</p>
				<div
					class="absolute top-1 left-0 -z-10 h-full w-full rounded-xl {!done && 'bg-[#7b1113]'}"
				/>
				<div
					class="{current
						? 'visible'
						: 'hidden'} absolute top-3 right-3 rounded-full bg-[#7b1113] px-4 py-0.5 text-white"
				>
					Ongoing
				</div>
			</div>
		{/each}
	</div>
</section>

<style lang="postcss"></style>
