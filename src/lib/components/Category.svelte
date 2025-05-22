<script lang="ts">
	import Heading from '$lib/components/Heading.svelte'

	let { title } = $props()
	// set lowercase and replace spaces with dashes
	const slug = title.toLowerCase().replace(/\s+/g, '-')
</script>

<Heading><h2 id={slug} class="text-2xl">{title}</h2></Heading>
