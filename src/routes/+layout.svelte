<script lang="ts">
	import './layout.css';
	import headshot from '$lib/assets/headshot.png';
	import GithubIcon from '@iconify-svelte/line-md/github';
	import TwitterIcon from '@iconify-svelte/line-md/twitter';
	import LinkedinIcon from '@iconify-svelte/line-md/linkedin';
	import EmailIcon from '@iconify-svelte/line-md/email';


	let { children } = $props();
</script>

<svelte:head>
	<title>Arman Pathan</title>
	<link rel="icon" href={headshot} />
</svelte:head>
{@render children()}

<!-- Minimalist right-side social column using Iconify (line-md) -->
<div class="hidden lg:flex fixed right-6 top-0 bottom-0 flex-col items-center justify-between z-50 pointer-events-none gap-3" aria-hidden="false">
	<!-- Top line -->
	<div class="w-1 grow bg-gray-600 mt-6 pointer-events-auto m"></div>

	<!-- Icons centered between top and bottom lines -->
	<nav class="flex flex-col items-center gap-3 pointer-events-auto" role="navigation" aria-label="Social links">
		<a class="text-gray-600 hover:text-gray-900 transition-colors" href="https://github.com/FigmentBoy" target="_blank" rel="noopener noreferrer" aria-label="GitHub">
			<GithubIcon height="2rem" />
		</a>

		<a class="text-gray-600 hover:text-gray-900 transition-colors" href="https://twitter.com/FigmentBoy_" target="_blank" rel="noopener noreferrer" aria-label="Twitter">
			<TwitterIcon height="2rem" />
		</a>

		<a class="text-gray-600 hover:text-gray-900 transition-colors" href="https://www.linkedin.com/in/arman-pathan-ap31" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn">
			<LinkedinIcon height="2rem" />
		</a>

		<a class="text-gray-600 hover:text-gray-900 transition-colors my-1" href="mailto:pathana@purdue.edu" target="_blank" rel="noopener noreferrer" aria-label="Email">
			<EmailIcon height="2rem" />
		</a>
	</nav>

	<!-- Bottom line -->
	<div class="w-1 h-14 bg-gray-600 mb-6 pointer-events-auto"></div>
</div>

