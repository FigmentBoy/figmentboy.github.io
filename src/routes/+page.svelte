<script lang="ts">
	import headshot from '$lib/assets/headshot.png';
	import GithubIcon from '@iconify-svelte/line-md/github';
	import TwitterIcon from '@iconify-svelte/line-md/twitter';
	import LinkedinIcon from '@iconify-svelte/line-md/linkedin';
	import EmailIcon from '@iconify-svelte/line-md/email';
</script>

<main class="min-h-screen">
	<div class="max-w-6xl mx-auto px-6 py-0 flex flex-col lg:flex-row lg:items-start gap-12">
		<!-- Hero (fills viewport height on large screens) -->
		<section id="hero" class="lg:w-1/2 flex items-center h-screen lg:sticky top-0">
			<div class="flex items-center gap-6 w-full">
				<!-- Picture -->
				<div class="flex-shrink-0">
					<img src={headshot} alt="Headshot" class="w-28 h-28 sm:w-36 sm:h-36 rounded-full object-cover shadow-sm" />
				</div>

				<!-- Name and CTA -->
				<div class="flex-1">
					<h1 class="text-3xl sm:text-4xl font-semibold text-gray-900">Arman Pathan</h1>
					<p class="mt-2 text-gray-600">I'm studying Computer Science and Mathematics at <span class="text-purdue">Purdue University</span> while refining my skills in Computer Graphics, Software Engineering, and Binary Analysis.</p>

					<!-- mobile: social icons above CTA -->
					<div class="flex items-center gap-4 mt-4 lg:hidden">
						<a class="text-gray-600 hover:text-gray-900 transition-colors" href="https://github.com/FigmentBoy" target="_blank" rel="noopener noreferrer" aria-label="GitHub">
							<GithubIcon height="1.4rem" />
						</a>
						<a class="text-gray-600 hover:text-gray-900 transition-colors" href="https://twitter.com/FigmentBoy_" target="_blank" rel="noopener noreferrer" aria-label="Twitter">
							<TwitterIcon height="1.4rem" />
						</a>
						<a class="text-gray-600 hover:text-gray-900 transition-colors" href="https://www.linkedin.com/in/arman-pathan-ap31" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn">
							<LinkedinIcon height="1.4rem" />
						</a>
						<a class="text-gray-600 hover:text-gray-900 transition-colors" href="mailto:pathana@purdue.edu" target="_blank" rel="noopener noreferrer" aria-label="Email">
							<EmailIcon height="1.4rem" />
						</a>
					</div>

					<a href="#projects" class="inline-block mt-4 text-sm text-gray-600 px-4 py-2 rounded hover:bg-gray-50 lg:hidden">View projects/skills →</a>
				</div>
			</div>
		</section>

		<!-- Projects: sits to the right on large screens and scrolls with the page -->
		<section id="projects" class="lg:w-1/2 bg-white">
			<div class="max-w-none mx-0 lg:mr-12 py-6 lg:py-12">
				<h2 class="text-2xl font-semibold">Projects</h2>
				<div class="mt-2 mb-6 h-px w-10 bg-gray-300"></div>
				<div class="space-y-6">
					<article class="border-b border-gray-200 pb-5">
						<div class="flex items-start justify-between gap-4">
							<div>
								<div class="flex items-center gap-2">
									<h3 class="text-lg font-semibold">zBot</h3>
									<a
										href="https://github.com/FigmentBoy/zBot"
										target="_blank"
										rel="noopener noreferrer"
										aria-label="zBot GitHub repository"
										class="text-gray-500 hover:text-gray-800 transition-colors"
									>
										<GithubIcon height="1.1rem" />
									</a>
								</div>
								<p class="text-sm italic text-gray-600">C++, Stripe, Flask, HTML/CSS, reCAPTCHA, Python, discord.py</p>
							</div>
							<p class="text-sm text-gray-600 whitespace-nowrap">Jan 2021 - Present</p>
						</div>
						<ul class="mt-3 list-disc pl-5 text-sm text-gray-700 space-y-1">
							<li>Developed fully integrated video game modifications with custom device rights management</li>
							<li>Generated more than $26,000 in revenue through webstore with over 100,000 downloads</li>
							<li>Reverse engineered and modified compiled x86 Assembly code using IDA, developing skills in binary analysis</li>
						</ul>
					</article>

					<article class="border-b border-gray-200 pb-5">
						<div class="flex items-start justify-between gap-4">
							<div>
								<div class="flex items-center gap-2">
									<h3 class="text-lg font-semibold">GDWeb</h3>
									<a
										href="https://github.com/FigmentBoy/GDWeb"
										target="_blank"
										rel="noopener noreferrer"
										aria-label="GDWeb GitHub repository"
										class="text-gray-500 hover:text-gray-800 transition-colors"
									>
										<GithubIcon height="1.1rem" />
									</a>
								</div>
								<p class="text-sm italic text-gray-600">C++, GLSL, Emscripten, OpenGL, WebGL, HTML, TailwindCSS, Typescript, Svelte</p>
							</div>
							<p class="text-sm text-gray-600 whitespace-nowrap">Oct 2023 - Present</p>
						</div>
						<ul class="mt-3 list-disc pl-5 text-sm text-gray-700 space-y-1">
							<li>Developed online WebGL video game level previewer</li>
							<li>Wrote OpenGL wrapper completely from scratch to customize the rendering pipeline</li>
							<li>Ran proxy serverless functions to access game servers using Cloudflare Workers</li>
						</ul>
					</article>

					<article class="border-b border-gray-200 pb-5">
						<div class="flex items-start justify-between gap-4">
							<div>
								<div class="flex items-center gap-2">
									<h3 class="text-lg font-semibold">Geode SDK</h3>
									<a
										href="https://github.com/geode-sdk/geode"
										target="_blank"
										rel="noopener noreferrer"
										aria-label="Geode SDK GitHub repository"
										class="text-gray-500 hover:text-gray-800 transition-colors"
									>
										<GithubIcon height="1.1rem" />
									</a>
								</div>
								<p class="text-sm italic text-gray-600">C++, CMake</p>
							</div>
							<p class="text-sm text-gray-600 whitespace-nowrap">Mar 2022 - Present</p>
						</div>
						<ul class="mt-3 list-disc pl-5 text-sm text-gray-700 space-y-1">
							<li>Collaborated with a team of international developers to develop a Geometry Dash modding SDK</li>
							<li>Learned the basics of open-source software development, template metaprogramming, and software licensing</li>
						</ul>
					</article>

					<article class="border-b border-gray-200 pb-5">
						<div class="flex items-start justify-between gap-4">
							<div>
								<h3 class="text-lg font-semibold">FriskyTool</h3>
								<p class="text-sm italic text-gray-600">Flask, HTML/CSS, Python, discord.py</p>
							</div>
							<p class="text-sm text-gray-600 whitespace-nowrap">Mar 2020 - Mar 2021</p>
						</div>
						<ul class="mt-3 list-disc pl-5 text-sm text-gray-700 space-y-1">
							<li>Helped develop the Friskytool discord bot as a website and auxiliary bot developer, growing to over 30k servers</li>
						</ul>
					</article>

					<article class="border-b border-gray-200 pb-5">
						<div class="flex items-start justify-between gap-4">
							<div>
								<h3 class="text-lg font-semibold">Freelance Programming</h3>
								<p class="text-sm italic text-gray-600">Flask, HTML/CSS, Python, discord.py</p>
							</div>
							<p class="text-sm text-gray-600 whitespace-nowrap">Mar 2020 - Mar 2022</p>
						</div>
						<ul class="mt-3 list-disc pl-5 text-sm text-gray-700 space-y-1">
							<li>Received commission over the two year period</li>
						</ul>
					</article>

					<article class="border-b border-gray-200 pb-5">
						<div class="flex items-start justify-between gap-4">
							<div>
								<h3 class="text-lg font-semibold">HACScraper</h3>
								<p class="text-sm italic text-gray-600">Flask, MongoDB</p>
							</div>
							<p class="text-sm text-gray-600 whitespace-nowrap">Nov 2020</p>
						</div>
						<ul class="mt-3 list-disc pl-5 text-sm text-gray-700 space-y-1">
							<li>Developed the UI/UX and helped organize development of project for the HackTAMS 2020 Hackathon</li>
							<li>Collaborated with another developer using Git to work in parallel</li>
							<li>Recipient of the Best UI/UX award</li>
						</ul>
					</article>

					<article class="pb-2">
						<div class="flex items-start justify-between gap-4">
							<div>
								<h3 class="text-lg font-semibold">Speech Emulation for Paralyzed and Mute Patients (SEFPAMP)</h3>
								<p class="text-sm italic text-gray-600">Python, OpenCV</p>
							</div>
							<p class="text-sm text-gray-600 whitespace-nowrap">Mar 2019</p>
						</div>
						<ul class="mt-3 list-disc pl-5 text-sm text-gray-700 space-y-1">
							<li>Integrated computer vision models to allow communication through a user's morse-code blinks</li>
							<li>Developed CAD models for a pair of glasses to allow for portable use of the software</li>
						</ul>
					</article>
				</div>

				<section id="skills" class="mt-12">
					<h2 class="text-2xl font-semibold">Skills</h2>
					<div class="mt-2 mb-4 h-px w-10 bg-gray-300"></div>
					<div class="space-y-6">
						<article class="border-b border-gray-200 pb-5">
							<h3 class="text-lg font-semibold">Skillsets/Interests</h3>
							<p class="mt-2 text-sm text-gray-700">Software Engineering, Binary Analysis, Algorithmic Analysis, Computer Graphics</p>
						</article>

						<article class="border-b border-gray-200 pb-5">
							<h3 class="text-lg font-semibold">Languages</h3>
							<p class="mt-2 text-sm text-gray-700">C/C++, GLSL, Java, Python, JavaScript/TypeScript, HTML/CSS</p>
						</article>

						<article class="border-b border-gray-200 pb-5">
							<h3 class="text-lg font-semibold">Tools</h3>
							<p class="mt-2 text-sm text-gray-700">Git/GitHub, Unix Shell, Ghidra/IDA Pro, CMake, SQL, MongoDB, Emscripten</p>
						</article>

						<article class="pb-2">
							<h3 class="text-lg font-semibold">Frameworks/Libraries</h3>
							<p class="mt-2 text-sm text-gray-700">Stripe, React, Svelte, Flask, discord.py, reCAPTCHA, ImGUI, OpenGL, WebGL</p>
						</article>
					</div>
				</section>
			</div>
		</section>
	</div>
</main>
