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

<h1>DSC UPD Solutions Challenge</h1>
<p>
	The Diliman Solutions Challenge is the flagship event of the Google Developer Student Clubs UP
	Diliman. This event seeks to call all students to ideate, innovate, and integrate relevant and
	effective solutions to pressing issues in local communities and the country, through the use of
	Google technology. Experience Google technology firsthand and pave the way for the youth to build
	a better tomorrow.
</p>
{#each linkData as { link, text }}
	<a href={link}>{text}</a>
{/each}
