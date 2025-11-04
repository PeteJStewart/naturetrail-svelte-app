<script lang="ts">
	type SectionProps = { id: string; title: string; children: () => any };
	let { id, title, children }: SectionProps = $props(); // Svelte 5 $props
</script>

<section aria-labelledby={id}>
	<h2 {id}>{title}</h2>
	{@render children()}
</section>

<style>
	h2 {
		font-size: 1.3rem;
		margin: 2rem 0 0.5rem;
		line-height: 1.25;
	}
	p {
		margin: 0.6rem 0;
	}
	ul {
		margin: 0.4rem 0 0.9rem 1.25rem;
	}
	.summary {
		border: 1px dashed var(--ring);
		border-radius: 12px;
		padding: 0.9rem 1rem;
		margin: 1rem 0 2rem;
		color: var(--muted);
	}
</style>
