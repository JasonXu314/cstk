<script lang="ts">
	export let title: string = '',
		description: string = '',
		links: Record<string, string> = {};
</script>

<article class="tool">
	<header>
		<slot name="head">
			<h1>{title}</h1>
		</slot>
	</header>
	<slot><p>{description}</p></slot>
	<footer>
		<slot name="foot">
			<div class="links">
				{#each Object.entries(links) as [alias, href]}
					<a {href}>
						{alias}
					</a>
				{/each}
			</div>
		</slot>
	</footer>
</article>

<style lang="scss">
	.tool {
		margin-top: 0;

		header h1 {
			margin-bottom: 0;
		}

		.links a {
			margin-right: 1em;
		}
	}
</style>
