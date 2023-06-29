<main class="container">
	<hgroup>
		<h1 class="title">
			This is the <span class="acrostic">
				<span class="word"><span class="lead">C</span>omp</span>
				<span class="word"><span class="lead">S</span>ci</span>
				<span class="word"><span class="lead">T</span>ool</span>
				<span class="word"><span class="lead">K</span>it.</span>
			</span>
		</h1>
		<h2>Or, conveniences that the school really ought to provide us but since it doesn't here they are as my own projects :D</h2>
	</hgroup>

	<section class="tools">
		<div class="grid">
			<article class="tool">
				<header>
					<h1>ER Diagram</h1>
				</header>
				<div class="grid">
					<img src="er-diagram-preview.png" alt="Preview" />
					<p>
						A tool that lets you build CS2300-compliant ER Diagrams, without the monetary pain of paid tools, or the psychological pain of using
						google drawings.
					</p>
				</div>
				<footer>
					<div class="links">
						<a href="https://cstk.jasonxu.dev/er">Link</a>
						<a href="https://github.com/JasonXu314/er-diagram" target="_blank" rel="noreferrer noopener">Repo</a>
					</div>
				</footer>
			</article>
			<article class="tool">
				<header>
					<h1>Simon Board Music</h1>
				</header>
				<div class="grid">
					<img src="music-maker-preview.png" alt="Preview" />
					<p>
						A tool that compiles sheet music into a format recognizable by the CLI to turn into ATMega C code. Support for assembly is coming
						soon&trade;.
					</p>
				</div>
				<footer>
					<div class="links">
						<a href="https://cstk.jasonxu.dev/music">Link</a>
						<a href="https://github.com/JasonXu314/ce3150-music" target="_blank" rel="noreferrer noopener">CLI</a>
						<a href="https://github.com/JasonXu314/ce3150-music-gui" target="_blank" rel="noreferrer noopener">Repo</a>
					</div>
				</footer>
			</article>
		</div>
		<div class="grid">
			<article class="tool">
				<header>
					<h1>G--</h1>
				</header>
				<p>
					A wrapper around the g++ compiler that does source analysis to automatically detect the c++ files that should be built for your program
					(assuming CS1570 conventions).
				</p>
				<footer>
					<div class="links">
						<a href="cbt" download="cbt">Download</a>
						<a href="https://github.com/JasonXu314/g--" target="_blank" rel="noreferrer noopener">Repo</a>
					</div>
				</footer>
			</article>
			<article class="tool">
				<header>
					<h1>CBT (WIP)</h1>
				</header>
				<p>
					<span class="abbr">C</span>(++) <span class="abbr">B</span>uild <span class="abbr">T</span>ool (😝). My experimental (and also very WIP)
					C++ package manager + build tool, all wrapped into one, built with plain from-scratch C++.
					<br />
					<br />
				</p>
				<footer>
					<div class="links">
						<a href="https://github.com/JasonXu314/ce3150-music-gui" target="_blank" rel="noreferrer noopener">Coming Soon</a>
					</div>
				</footer>
			</article>
		</div>
		<div class="grid">
			<article class="tool">
				<header>
					<h1>Coming Soon</h1>
				</header>
				<p>
					There are other tools in the works: in particular, a tool similar to the ER Diagram tool but for relational diagrams (or an add-on for that
					tool).
				</p>
				<footer>
					<div class="links">
						<a href="https://github.com/JasonXu314">My GitHub :D</a>
					</div>
				</footer>
			</article>
		</div>
	</section>
</main>

<svelte:head>
	<title>CSTK</title>
</svelte:head>

<style lang="scss">
	.title {
		.acrostic {
			display: inline-flex;
			flex-direction: column;

			.word {
				margin-top: -0.3lh;

				.lead {
					color: var(--primary);
				}
			}
		}
	}

	.tool {
		margin-top: 0;

		header h1 {
			margin-bottom: 0;
		}

		footer {
			display: block;
			margin-top: auto;
		}

		.links a {
			margin-right: 1em;
		}

		.abbr {
			color: var(--primary);
		}
	}
</style>
