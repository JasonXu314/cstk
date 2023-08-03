<script>
	import Tool from './Tool.svelte';
</script>

<main class="container">
	<hgroup>
		<h1 class="title">
			This is the <span class="acrostic">
				<span class="word">Comp</span>
				<span class="word">Sci</span>
				<span class="word">Tool</span>
				<span class="word">Kit.</span>
			</span>
		</h1>
		<h2>Or, conveniences that the school really ought to provide us but since it doesn't here they are as my own projects :D</h2>
	</hgroup>

	<section class="tools">
		<div class="grid">
			<Tool title="ER Diagram">
				<div class="grid">
					<img class="preview" src="er-diagram-preview.png" alt="Preview" />
					<p>
						A tool that lets you build CS2300-compliant ER Diagrams, without the monetary pain of paid tools, or the emotional pain of google
						drawings.
					</p>
				</div>
				<div class="links" slot="foot">
					<a href="https://cstk.jasonxu.dev/er">Link</a>
					<a href="https://github.com/JasonXu314/er-diagram" target="_blank" rel="noreferrer noopener">
						<i class="fa-solid fa-arrow-up-right-from-square fa-xs" />
						Repo
					</a>
				</div>
			</Tool>
			<Tool title="Simon Board Music">
				<div class="grid">
					<img class="preview" src="music-maker-preview.png" alt="Preview" />
					<p>
						A GUI tool that compiles sheet music into a format recognizable by the CLI to turn into ATMega32 C code. Support for assembly is Coming
						Soon&trade;.
					</p>
				</div>
				<div class="links" slot="foot">
					<a href="https://cstk.jasonxu.dev/music">GUI</a>
					<a
						href="simony"
						download="simony"
						data-tooltip={'A bad pun on "Simon" and "harmony" that actually means the selling of church titles lol'}
					>
						<i class="fa-solid fa-download fa-xs" />
						CLI Download
					</a>
					<a href="https://github.com/JasonXu314/ce3150-music" target="_blank" rel="noreferrer noopener">
						<i class="fa-solid fa-arrow-up-right-from-square fa-xs" />
						CLI Repo
					</a>
					<a href="https://github.com/JasonXu314/ce3150-music-gui" target="_blank" rel="noreferrer noopener">
						<i class="fa-solid fa-arrow-up-right-from-square fa-xs" />
						GUI Repo
					</a>
				</div>
			</Tool>
		</div>
		<div class="grid">
			<Tool title="Relational Diagram">
				<div class="grid">
					<img class="preview" src="rel-diagram-preview.png" alt="Preview" />
					<p>A tool that lets you build CS2300-compliant Relational Diagrams.</p>
				</div>
				<div class="links" slot="foot">
					<a href="https://cstk.jasonxu.dev/rel">Link</a>
					<a href="https://github.com/JasonXu314/relational-diagram" target="_blank" rel="noreferrer noopener">
						<i class="fa-solid fa-arrow-up-right-from-square fa-xs" />
						Repo
					</a>
				</div>
			</Tool>
			<Tool title="JSFlap">
				<div class="grid">
					<img class="preview" src="jsflap-preview.png" alt="Preview" />
					<p>A (kind of incomplete) JFlap clone with backwards compatibility for building & testing FSMs more easily.</p>
				</div>
				<div class="links" slot="foot">
					<a href="https://cstk.jasonxu.dev/jsflap">Link</a>
					<a href="https://github.com/JasonXu314/jsflap" target="_blank" rel="noreferrer noopener">
						<i class="fa-solid fa-arrow-up-right-from-square fa-xs" />
						Repo
					</a>
				</div>
			</Tool>
		</div>
		<div class="grid">
			<Tool
				title="G--"
				description="A wrapper around the g++ compiler that does source analysis to automatically detect the C++ files that should be built for your program
			(assuming CS1570 conventions)."
			>
				<div class="links" slot="foot">
					<a href="g--" download="g--">
						<i class="fa-solid fa-download fa-xs" />
						Download
					</a>
					<a href="https://github.com/JasonXu314/g--" target="_blank" rel="noreferrer noopener">
						<i class="fa-solid fa-arrow-up-right-from-square fa-xs" />
						Repo
					</a>
				</div>
			</Tool>
			<Tool title="🛠️ CBT (WIP)">
				<p>
					<span class="abbr">C</span>(++) <span class="abbr">B</span>uild <span class="abbr">T</span>ool. My experimental (and also very WIP) C++
					package manager + build tool, all wrapped into one, built with plain from-scratch C++.
				</p>
				<div class="links" slot="foot">
					<a href="/">
						<i class="fa-solid fa-screwdriver-wrench fa-xs" />
						Coming Soon
					</a>
				</div>
			</Tool>
		</div>
		<div class="grid">
			<Tool title="🚀 Coming Soon" description="There are other tools & enhancements in the works, keep an eye out for changes!">
				<div class="links" slot="foot">
					<a href="https://github.com/JasonXu314" target="_blank" rel="noreferrer noopener">
						<i class="fa-solid fa-arrow-up-right-from-square fa-xs" />
						My GitHub 🙂
					</a>
				</div>
			</Tool>
		</div>
	</section>
</main>

<svelte:head>
	<title>CSTK</title>
	<meta name="author" content="Jason Xu" />
	<meta name="description" content="A collection of tools/utilities to make CS at MST just a bit more bearable :)" />
	<meta name="keywords" content="computer science,utilities" />
	<meta property="og:locale" content="en_US" />
	<meta property="og:type" content="website" />
	<meta property="og:title" content="Home" />
	<meta property="og:description" content="A collection of tools/utilities to make CS at MST just a bit more bearable :)" />
	<meta property="og:url" content="https://cstk.jasonxu.dev" />
	<meta property="og:site_name" content="CSTK (Comp Sci Tool Kit)" />
	<meta property="og:image" content="https://jasonxu.dev/logo.png" />
	<meta name="theme-color" content="#1897C2" />
</svelte:head>

<style lang="scss">
	.title {
		.acrostic {
			display: inline-flex;
			flex-direction: column;

			.word {
				margin-top: -0.3lh;

				&::first-letter {
					color: var(--primary);
				}
			}
		}
	}

	:global(.tool) {
		margin-top: 0;

		.links a {
			margin-right: 1em;

			i {
				vertical-align: 50%;
			}
		}

		.abbr {
			color: var(--primary);
		}

		.grid {
			gap: 1rem;
		}

		.preview {
			max-height: 6lh;
		}
	}
</style>
