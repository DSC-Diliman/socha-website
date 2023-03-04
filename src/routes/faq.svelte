<script>
	let faq = [
		{
			section: 'General',
			questions: [
				{
					q: "What's this event about?",
					a: 'The Diliman Solutions Challenge is a nationwide Google hackathon event that focuses on using Google technology to ideate, develop, and innovate a solution in relation with one of the UN Sustainable Development Goals'
				},
				{
					q: 'What are the 17 Sustainable Development Goals of the United Nations? Can my solution solve a problem outside the scope of the 17 SDGs?',
					a: 'Created by the United Nations in 2015 and to be achieved by 2030, the 17 Sustainable Development Goals (SDGs) agreed upon by all 193 United Nations Member States aim to end poverty, ensure prosperity, and protect the planet. More information about the 17 SDGs can be found in the link attached to the photo. We require your submitted solution to solve for at least one or more of the 17 Sustainable Development Goals (SDGs), which you will be indicating when you submit your proposals.'
				},
				{
					q: 'What Google developer tools are we required to use?',
					a: 'Use one or more Google products or platforms including, but not limited to: Android, Angular, Google Cloud (Serverless functions, Kubernetes, ML services, Data engg), Firebase, Google Maps Platform, Tensorflow, Progressive Web Apps, Flutter, Assistant / Actions on Google'
				},
				{
					q: 'Where will be event be held?',
					a: 'The event will primarily be using Zoom and Discord for most of our synchronous sessions, while the face to face Demo Day will be around the UP Diliman area. The exact location will be announced a week prior to Demo Day.'
				},
				{
					q: 'What is the difference between the Diliman Solutions Challenge and the global Solutions Challenge?',
					a: 'Participation in the Diliman Solutions Challenge is only limited to Filipinos and teams with at least one UP Diliman student. The global Solutions Challenge is open to all people of any field and profession.'
				}
			]
		},
		{
			section: 'Registration',
			questions: [
				{
					q: "I want to join but I don't have a team yet. Will you be able to help me with this?",
					a: 'Yes! We group together individuals who have not yet formed a team with other individuals or groups who still lack a few members based on the different needs of the team. We will be releasing a list of of the team groupings before the start of the ideathon.'
				},
				{
					q: 'Is there a particpation fee or is it free?',
					a: 'This event does not have a participation or registration fee.'
				},
				{
					q: "Can I join if I'm not from UP Diliman? Or can my team join if one or more of us are not from UP Diliman?",
					a: 'Yes, as long as at least one member of your team is from UP Diliman, your team can participate in the Diliman Solutions Challenge.'
				},
				{
					q: "Can I join if I'm not a student? Or can my team join if one or more of us are not students?",
					a: 'Yes, just as long as at least one of your team members is.'
				},
				{
					q: 'Where do I sign up?',
					a: 'You may register individually or as a team through this link: bit.ly/SolCha23_RegForm'
				}
			]
		},
		{
			section: 'Ideation & Workshop',
			questions: [
				{
					q: 'Do I need a working prototype after the event?',
					a: 'No. All you need is the proposal after submission, but it must discuss how you will include your Google Technology.'
				},
				{
					q: 'Do I need to know how to code to join this event?',
					a: 'No, though it is encouraged that you have someone in your team that does, especially since the proposal requires you to indicate how you incorporate Google technologies. We have provided resources on these topics that you may use as references throughout the event proper.'
				},
				{
					q: 'Can one participant or team submit multiple proposals if they contributed to both projects?',
					a: 'No. We will limit one (1) proposal submission per person, so they can only be a part of one submission.'
				},
				{
					q: 'Am I required to participate in the workshops?',
					a: 'No, but it is highly encouraged as it would help you think about how to incorporate Google technologies in your solution.'
				},
				{
					q: "I want to attend the workshops, but I won't be free...",
					a: 'A recording of our session will be sent in the Discord server for your reference.'
				},
				{
					q: "If I'm not participating in the main event, can I still attend the workshops?",
					a: 'Our recorded livestreams will be available to the general public, but the Zoom meeting will be accessible only to participants.'
				},
				{
					q: 'Do I need to be good at coding to attend the workshops?',
					a: "Not at all! This is a learning session, and so we encourage people who don't know how to do these to participate."
				}
			]
		},
		{
			section: 'Mentorship & Prototyping',
			questions: [
				{
					q: 'Will all teams reach this week?',
					a: 'An elimination will occur throughout the week. For teams to reach this stage, they need to go through all weeks.'
				},
				{
					q: 'Do I need to consult with my mentor?',
					a: ''
				},
				{
					q: "We used other non-Google developer tools to create our prototype in addition to Google's developer tools. Is that allowed?",
					a: 'Yes. We only require that your submissions use at least one of the Google products or platforms, but you are allowed to use other tools if necessary.'
				},
				{
					q: 'How will submission go?',
					a: 'Though subject to change, submissions will be conducted through Google Forms and verified through email.'
				},
				{
					q: 'How many minutes should the Audio Visual Presentation be?',
					a: 'All AVPs should be a maximum of 2 minutes explaining what your innovation is all about, a walk through of your prototype, and what impact it can bring to your target community'
				}
			]
		},
		{
			section: 'Demo Day',
			questions: [
				{
					q: 'When is Demo Day?',
					a: 'Our face to face Demo Day will be on March 25 from 1PM to 6PM.'
				},
				{
					q: 'What if I cannot attend Demo Day face to face?',
					a: 'Teams who are unable to pitch their innovations live can pitch via Zoom, which will be streamed to the live audience present in the venue of the face to face demo day.'
				}
			]
		}
	];
</script>

<h1 id="faq">Frequently Asked Questions</h1>
{#each faq as { section, questions }}
	<h2>{section}</h2>
	{#each questions as { q, a }}
		<h3>{q}</h3>
		<div>{a}</div>
	{/each}
{/each}

<style lang="postcss"></style>
