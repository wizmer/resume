<script lang="ts">
	const experiences = [
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
</script>

<section class="experiences">
	<h2>Professional Experience</h2>
	{#each experiences as experience}
		<article class="experience">
			<header>
				<div class="title-container">
					<h3>{experience.role}</h3>
					<div class="company">{experience.company}</div>
				</div>
				<div class="meta">
					<span class="period">{experience.period}</span>
					<span class="location">{experience.location}</span>
				</div>
			</header>
			<ul class="description">
				{#each experience.description as item}
					<li>{item}</li>
				{/each}
			</ul>
			<footer class="technologies">
				{#each experience.technologies as tech}
					<span class="tech-tag">{tech}</span>
				{/each}
			</footer>
		</article>
	{/each}
</section>

<style>
	.experiences {
		max-width: 900px;
		margin: 0 auto;
		padding: 1rem;
	}

	.experience {
		margin-bottom: 2rem;
		padding-bottom: 2rem;
		border-bottom: 1px solid #eee;
	}

	.experience header {
		display: flex;
		justify-content: space-between;
		align-items: flex-start;
		margin-bottom: 1rem;
	}

	.title-container h3 {
		margin: 0;
		color: #2c3e50;
	}

	.company {
		color: #666;
		font-weight: 500;
	}

	.meta {
		text-align: right;
		color: #666;
	}

	.period,
	.location {
		display: block;
	}

	.description {
		margin: 1rem 0;
		padding-left: 1.5rem;
	}

	.description li {
		margin-bottom: 0.5rem;
	}

	.technologies {
		display: flex;
		flex-wrap: wrap;
		gap: 0.5rem;
		margin-top: 1rem;
	}

	.tech-tag {
		background: #f0f0f0;
		padding: 0.25rem 0.75rem;
		border-radius: 15px;
		font-size: 0.875rem;
		color: #666;
	}
</style>
