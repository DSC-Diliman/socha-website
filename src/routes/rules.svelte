<script lang="ts">
	interface Subsection {
		subtitle: string;
		submarks: string;
		criteria: string[];
	}

	interface Section {
		title: string;
		marks: string;
		subsections: Subsection[];
	}

	let colors = ['bg-red-500', 'bg-yellow-500', 'bg-emerald-500'];

	let additionalRules = [
		'Please upload your documents in GitHub.',
		'Provide instructions on how to run, compile, and execute your projects.',
		'Add dscdiliman@gmail.com as a collaborator.',
		'If you have any inquiries, please message Zoe Huertas, Kurt Lanting, or any of the organizers.'
	];

	let scoring: Section[] = [
		{
			title: 'Innovation Proposal (Idea)',
			marks: '50%',
			subsections: [
				{
					subtitle: 'The Idea',
					submarks: '15%',
					criteria: [
						'Provides a unique and intuitive approach in the problem.',
						'Discusses at least 1 UN SDG and provides relevance in the context of the Philippines.',
						'Data-driven and evidence-based solution.'
					]
				},
				{
					subtitle: 'Clarity',
					submarks: '10%',
					criteria: [
						'Clearly communicates the purpose, objective, and necessity of the project.',
						'Concise and straightforward with the message of the text.',
						'Does not exceed more than 7 pages in text pages (not including Cover, References, & Appendix).'
					]
				},
				{
					subtitle: 'Impact',
					submarks: '10%',
					criteria: [
						'The target SDG and the local issue are contextualized well enough to convince relevance.',
						'The market study is well-identified and is placed as a major stakeholder of the project.',
						'The idea presents a tangible and significant impact on the stakeholders.'
					]
				},
				{
					subtitle: 'Resources',
					submarks: '5%',
					criteria: [
						'Provides data-backed information (At least 5 credible resources).',
						'APA Citation-- utilizes in-text citation.'
					]
				},
				{
					subtitle: 'Google Technology',
					submarks: '10%',
					criteria: [
						'Comprehensive discussion on how Google Technologies will be used.',
						'Appropriateness of the Technology used.'
					]
				}
			]
		},
		{
			title: 'Prototype (Technology)',
			marks: '30%',
			subsections: [
				{
					subtitle: 'Translation of Ideas',
					submarks: '9%',
					criteria: [
						'Ideas presented in the Innovation proposal are expressed and are well executed in the Prototype.',
						'There is a clear objective to the application.',
						'Prototype addresses the main issue (SDG) and is impactful.'
					]
				},
				{
					subtitle: 'User Experience',
					submarks: '4½%',
					criteria: [
						'Considers the experience of users in terms of usability and interface (With backed data to support claims).',
						'Prototype is easy to understand, use, and follow.',
						'A guide is present on how to navigate the Hi-Fidelity Mock-Ups. '
					]
				},
				{
					subtitle: 'Google Technology',
					submarks: '10½%',
					criteria: [
						'While the Coded solution is not required, a 3% allotment will be given to teams who provide coded solutions.',
						'Comprehensively discuss how Google Technology is used and how it is utilized.',
						'The usage of Google Technology can be seen in the Prototype itself.'
					]
				},
				{
					subtitle: 'Hi-Fidelity',
					submarks: '6%',
					criteria: [
						'Provides Hi-Fi mock-ups for the prototype.',
						'Takes note of design principles and presents an interactive interface for the project.'
					]
				}
			]
		},
		{
			title: 'Audio-Visual Presentation Demo (Pitch)',
			marks: '20%',
			subsections: [
				{
					subtitle: 'Video',
					submarks: '6%',
					criteria: [
						'Video is comprehensive, elaborate, and appropriate for the audience.',
						'Video is relevant to the topic and discusses the Prototype and the project holistically.',
						'Video is compelling and impactful.'
					]
				},
				{
					subtitle: 'Live Presentation',
					submarks: '6%',
					criteria: [
						'The live presentation is straightforward and elaborate.',
						'Provides a brief background, but focuses on the demo of the Prototype.',
						'Provides a clear and elaborate discussion on how the prototype works and how it addresses its objectives.',
						'Presenter/s effectively and clearly explains all features and functionalities of the product.'
					]
				},
				{
					subtitle: 'Demo - Google Tech',
					submarks: '6%',
					criteria: [
						'Shows the actual prototype being demo-ed on screen.',
						'Covers all the functionalities and points of inquiry of the prototype with regard to usage and Google Technology.',
						'Effectively conveys how the product is to be used by its users and how it will impact the stakeholders.'
					]
				},
				{
					subtitle: 'Instructions',
					submarks: '2%',
					criteria: [
						'Follows the 2-min guidelines.',
						'Hosted in YouTube (Allowed to be unlisted)',
						'Follows the format title (_Solution Name_ - _Team Name_ - Diliman Solutions Challenge 2023)'
					]
				}
			]
		}
	];
</script>

<section class="py-20 px-8" id="rules">
	<h1 class="mb-10 text-center text-6xl font-bold">Rules</h1>

	<div class="sm:mx-12 lg:mx-24">
		<h2 class="mb-5 text-4xl">Eligibility</h2>
		<p class="mb-10">
			This competition is open to individuals or teams of university students regardless of academic
			background. A team may have a maximum of 4 members.
		</p>

		<h2 class="mb-5 text-4xl">Scoring</h2>
		<div class="mb-10">
			{#each scoring as { title, marks, subsections }, index}
				<div class="mb-10">
					<div class="flex items-center gap-3">
						<p
							class="flex h-12 w-12 items-center justify-center rounded-full font-bold {colors[
								index
							]} text-white"
						>
							{marks}
						</p>
						<h3>{title}</h3>
					</div>
					{#each subsections as { subtitle, submarks, criteria }}
						<div class="my-6">
							<div class="ml-12 flex items-center gap-3">
								<p
									class="flex h-12 w-12 items-center justify-center rounded-full bg-[#7b1113] text-white"
								>
									{submarks}
								</p>
								<h4>{subtitle}</h4>
							</div>
							<ul class="ml-28 my-3 list-disc">
								{#each criteria as criterion}
									<li>{criterion}</li>
								{/each}
							</ul>
						</div>
					{/each}
				</div>
			{/each}
		</div>

		<h2 class="mb-5 text-4xl">Additional Rules</h2>
		<ul class="list-disc">
			{#each additionalRules as additionalRule}
				<li class="ml-5">{additionalRule}</li>
			{/each}
		</ul>
	</div>
</section>

<style lang="postcss"></style>
