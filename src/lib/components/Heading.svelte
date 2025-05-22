<script lang="ts">
	interface HeadingProps {
		children: any
		class?: string
		variant?: 'default' | 'dark' | 'light'
	}
	let { children, class: className, variant = 'default' }: HeadingProps = $props()
</script>

<div class={['flex flex-wrap items-center gap-3 py-3', className]}>
	{@render bar()}
	{@render children()}
	{@render bar(true)}
</div>

{#snippet bar(invert = false)}
	<div
		class={[
			'flex w-6 items-center last:grow',
			variant === 'dark' && '*:bg-emerald-950',
			variant === 'default' && '*:bg-emerald-900',
			variant === 'light' && '*:bg-emerald-800'
		]}
	>
		<div class="h-1 grow"></div>
		<div class="aspect-square h-3" class:order-first={invert}></div>
	</div>
{/snippet}
