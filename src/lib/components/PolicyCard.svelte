<script lang="ts">
	let { children } = $props(); // Svelte 5 $props
</script>

<article class="card" role="article">
	{@render children()}
</article>

<style>
	.card {
		background: var(--card);
		border: 1px solid var(--ring);
		border-radius: var(--radius);
		padding: clamp(1rem, 2vw + 0.5rem, 2rem);
	}
</style>
