<script>
	let events = [
		{
			duration: 'February 18 - March 5',
			event: 'REGISTRATION PERIOD',
			description:
				'Registration period will be open for over two weeks. Participants may register here.'
		},
		{
			duration: 'February 20 - March 4',
			event: 'INTERACT: NETWORKING AVENUES',
			description: 'Meet and network with other participants through the event Discord channel.'
		},
		{
			duration: 'March 4 - 5',
			event: 'IDEATE: 48-HOUR IDEATHON CHALLENGE',
			description:
				'A 48-hour intensive brainstorming session to come up with an innovation proposal along with activities to help the ideation process.'
		},
		{
			duration: 'March 11 - 19',
			event: 'INNOVATE: PROTOTYPING PERIOD & MENTORSHIP SESSIONS',
			description:
				"This is the beginning of the team's prototype creation. The mentorship sessions are designed to guide teams in creating a successful prototype of their idea and preparing for a live pitch and an AVP. Teams receive feedback and consultations from mentors to refine their proposals and increase their chances of success for their final submissions."
		},
		{
			duration: 'March 25',
			event: 'IMPLEMENT: LIVE PITCHING DEMO DAY',
			description:
				'A 48-hour intensive brainstorming session to come up with an innovation proposal along with activities to help the ideation process.'
		},
		{
			duration: 'March 25',
			event: 'AWARDING CEREMONY',
			description:
				'On the same day of the live pitching, winners will be announced. Do you have what it takes to reach the top?'
		}
	];
</script>

<h1 id="timeline">Timeline</h1>
{#each events as { duration, event, description }}
	<p>{duration}</p>
	<h2>{event}</h2>
	<p>{description}</p>
{/each}

<style lang="postcss"></style>
