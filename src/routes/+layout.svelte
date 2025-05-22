<script lang="ts">
	import '../app.css'

	let { children } = $props()
</script>

<div
	class="flex min-h-screen flex-col divide-y-4 divide-emerald-900 md:flex-row md:divide-x-4 md:divide-y-0"
>
	{@render children()}
</div>
