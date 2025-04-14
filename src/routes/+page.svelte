<script lang="ts">
	const experiences = [
		{
			company: 'Peachtree Infrastructure',
			role: 'Technical Lead',
			period: '2022 - Present',
			location: 'Remote',
			description: [
				'Led development of an IoT platform managing temperature control across large building fleets',
				'Designed and implemented real-time thermostat monitoring and control system',
				'Built scalable architecture to handle thousands of connected devices',
				'Optimized energy consumption through smart temperature management algorithms'
			],
			technologies: [
				'Python',
				'Svelte',
				'TypeScript',
				'Google Cloud Platform',
				'BigQuery',
				'Cloud SQL',
				'Cloud Tasks',
				'Cloud Scheduler',
				'Firebase',
				'Sequelize',
				'PostgreSQL',
				'Vitest',
				'Playwright'
			]
		},
		{
			company: 'PepsiCo Global',
			role: 'Python Engineer for a Data Science Team',
			period: '2021 - 2022',
			location: 'Remote',
			description: [
				'Supervised the refactoring of the codebase, set up CI and test framework. Optimized code performances and eliminated technical debt',
				'Developed new data analysis pipelines using Spark for clustering algorithms. Set up AWS buckets for computation caching',
				'Automated a manual workflow reducing task duration from one hour to five minutes',
				'Implemented Hydra for configuration management',
				'Designed a Python package for Jira board interaction with automated CLI history tracking'
			],
			technologies: [
				'Python',
				'SQL',
				'Pandas',
				'Spark',
				'PostgreSQL',
				'CI/CD',
				'Pytest',
				'AWS',
				'Data Engineering'
			]
		},
		{
			company: 'Blue Brain Project',
			role: 'Senior Scientific Developer',
			period: '2017 - 2021',
			location: 'Switzerland',
			description: [
				'Developed open-source Python/C++ I/O library for neuron morphology files',
				'Managed and modernized morphology stack (20+ libraries)',
				'Maintained PostgreSQL database for scientific artifact provenance tracking',
				'Led CI/CD implementation using Travis CI, Github, and Jenkins',
				'Built internal website using Django and Vue connected to Python packages'
			],
			technologies: [
				'Python',
				'C++',
				'PyBind11',
				'PostgreSQL',
				'Django',
				'Vue',
				'CI/CD',
				'NumPy',
				'Pandas',
				'GitHub API'
			]
		},
		{
			company: 'Amadeus',
			role: 'Python Back-end Developer',
			period: '2016 - 2017',
			location: 'France',
			description: [
				'Developed optimization algorithms for flight passenger reseating',
				'Maintained MySQL database for flight passenger management',
				'Performed on-call support for client airlines',
				'Contributed to front-end development using Angular'
			],
			technologies: ['Python', 'SQL', 'C++', 'AngularJS', 'MySQL', 'REST APIs']
		},
		{
			company: 'AMS',
			role: 'Post-Doctoral Researcher',
			period: '2014 - 2016',
			location: 'Switzerland',
			description: [
				'Analyzed cosmic-ray data using Bayesian techniques and machine learning',
				'Performed particle physics simulation for detector behavior analysis',
				'Implemented MCMC techniques for probability distribution sampling',
				'Managed communication between detector HQ and NASA HQ'
			],
			technologies: [
				'BigQuery',
				'ROOT',
				'NumPy',
				'Pandas',
				'Machine Learning',
				'Neural Networks',
				'MCMC',
				'Data Analytics'
			]
		},
		{
			company: 'Croustie',
			role: 'Founder and Full-stack Developer',
			period: '2014 - 2015',
			location: 'France',
			description: [
				'Developed mobile app and website for simplified grocery shopping',
				'Built Django-based website with recipe database integration',
				'Implemented web scraping for recipe collection and processing'
			],
			technologies: [
				'Django',
				'AngularJS',
				'SQLite',
				'Android',
				'Web Scraping',
				'Beautiful Soup',
				'REST APIs'
			]
		},
		{
			company: 'Optopartner',
			role: 'R&D Software Engineer',
			period: '2013 - 2014',
			location: 'France',
			description: [
				'Developed and maintained embedded communication software',
				'Debugged bus communication issues',
				'Coordinated between server and embedded device teams'
			],
			technologies: ['Embedded C', 'C++', 'Boost', 'CAN Bus']
		},
		{
			company: 'Joseph Fourier University',
			role: 'PhD Researcher',
			period: '2009 - 2012',
			location: 'France',
			description: [
				'Modeled physics simulation for cosmic ray detector analysis',
				'Performed data analysis of cosmic ray fluxes using Bayesian inference',
				'Implemented MCMC algorithm for galactic cosmic ray propagation parameters',
				'Published research findings in academic papers'
			],
			technologies: ['C++', 'ROOT', 'MCMC', 'Data Analytics', 'Data Visualization']
		}
	];

	import { fade } from 'svelte/transition';
</script>

<main class="mx-auto min-h-screen max-w-4xl bg-gradient-to-b from-gray-50 to-white p-4">
	<header class="mb-16 text-center">
		<h1
			class="mb-4 bg-gradient-to-r from-gray-900 to-gray-600 bg-clip-text text-5xl font-bold text-transparent"
		>
			Benoit Coste
		</h1>
		<h2 class="mb-4 text-2xl font-medium text-gray-700">Senior Software Engineer</h2>
		<div class="flex items-center justify-center gap-4 text-gray-600">
			<div class="flex items-center gap-2">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="h-5 w-5"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path
						fill-rule="evenodd"
						d="M5.05 4.05a7 7 0 119.9 9.9L10 18.9l-4.95-4.95a7 7 0 010-9.9zM10 11a2 2 0 100-4 2 2 0 000 4z"
						clip-rule="evenodd"
					/>
				</svg>
				<span>74100 Ambilly, FRANCE</span>
			</div>
			<a
				href="https://github.com/wizmer"
				target="_blank"
				rel="noopener noreferrer"
				class="flex items-center gap-2 transition-colors duration-300 hover:text-gray-800"
			>
				<svg class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
					<path
						d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"
					/>
				</svg>
				<span>GitHub</span>
			</a>
		</div>
	</header>

	<section class="mb-12">
		<h2 class="mb-6 text-2xl font-bold">Professional Experience</h2>
		{#each experiences as experience, i}
			<article
				in:fade={{ delay: i * 100, duration: 300 }}
				class="mb-8 rounded-lg border-b border-gray-200 p-6 pb-8 transition-all duration-300 last:border-0 hover:shadow-lg"
			>
				<header class="mb-4 flex items-start justify-between hover:text-gray-800">
					<div>
						<h3
							class="relative m-0 inline-block text-xl font-medium text-gray-800 after:block after:h-0.5 after:w-0 after:bg-gray-600 after:transition-all after:content-[''] hover:after:w-full"
						>
							{experience.role}
						</h3>
						<div class="font-medium text-gray-600">{experience.company}</div>
					</div>
					<div class="text-right text-gray-600">
						<span class="block">{experience.period}</span>
						<span class="block">{experience.location}</span>
					</div>
				</header>
				<ul class="my-4 ml-6 list-disc">
					{#each experience.description as item}
						<li class="mb-2 text-gray-700">{item}</li>
					{/each}
				</ul>
				<footer class="mt-4 flex flex-wrap gap-2">
					{#each experience.technologies as tech}
						<span class="tech">
							{tech}
						</span>
					{/each}
				</footer>
			</article>
		{/each}
	</section>

	<section class="mb-12">
		<h2 class="mb-6 text-2xl font-bold">Personal Interests</h2>
		<div class="grid gap-4 sm:grid-cols-2">
			<div
				class="rounded-lg bg-gradient-to-br from-green-50 to-gray-50 p-6 transition-all duration-300 hover:shadow-lg"
			>
				<div class="mb-2 flex items-center gap-2">
					<svg class="h-5 w-5 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M4 16l4.586-4.586a2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 0 012.828 0L20 14m-6-6h.01M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z"
						/>
					</svg>
					<h3 class="text-lg font-medium">Sustainable Mobility</h3>
				</div>
				<p class="text-gray-600">Enthusiast advocating for eco-friendly transportation solutions</p>
				<a
					href="https://envilleavelo.fr/"
					target="_blank"
					rel="noopener noreferrer"
					class="text-blue-600 hover:underline">En Ville à Vélo</a
				>
			</div>

			<div
				class="rounded-lg bg-gradient-to-br from-blue-50 to-gray-50 p-6 transition-all duration-300 hover:shadow-lg"
			>
				<div class="mb-2 flex items-center gap-2">
					<svg class="h-5 w-5 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M5 3v16M5 19h14l-7-14-2 4-5 10zm14 0V8"
						/>
					</svg>
					<h3 class="text-lg font-medium">Rock Climbing</h3>
				</div>
				<p class="text-gray-600">for the last 20 years</p>
				<ul class="ml-6 list-disc text-gray-600">
					<li>Lead climbing</li>
					<li>Multi-pitch climbing</li>
					<li>Bouldering</li>
				</ul>
			</div>
		</div>
	</section>
</main>

<style lang="postcss">
	@reference "tailwindcss";

	.tech {
		@apply transform rounded-full bg-gradient-to-r from-gray-100 to-gray-50 px-3 py-1 text-sm text-gray-600 transition-all duration-300 hover:-translate-y-0.5 hover:from-gray-200 hover:to-gray-100 hover:shadow-md;
	}
</style>
