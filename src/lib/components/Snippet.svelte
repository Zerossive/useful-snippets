<script lang="ts">
	let { children, title } = $props()
	const slug = title.toLowerCase().replace(/\s+/g, '-')
</script>

<section id={slug}>
	<h3 class=" px-3 text-lg text-emerald-400">{title}</h3>
	{@render children()}
</section>
