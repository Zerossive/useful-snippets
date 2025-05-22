<script lang="ts">
	import PixelarticonsCopy from '~icons/pixelarticons/copy'

	let codeBlock: HTMLDivElement

	let { code = '' } = $props()
	//remote leading and trailing empty newlines
	code = code.replace(/^\s*\n/, '').replace(/\n\s*$/, '')

	function handleCopy() {
		// copy children text to clipboard
		navigator.clipboard.writeText(code)

		// run animation on code block to indicate copy success
		const toggledClassList = ['brightness-125']
		codeBlock.classList.add(...toggledClassList)
		setTimeout(() => {
			codeBlock.classList.remove(...toggledClassList)
		}, 300)
	}
</script>

<div
	class="my-6 flex w-full flex-wrap items-start bg-emerald-900 duration-150"
	bind:this={codeBlock}
>
	<pre class="grow overflow-x-auto px-4 py-2"><code class="">{code}</code></pre>
	<button
		class="group flex w-full cursor-pointer items-center justify-center bg-emerald-800 p-2 duration-75 hover:bg-emerald-700 md:w-auto"
		onclick={handleCopy}
		aria-label="copy code snippet to clipboard"
	>
		<PixelarticonsCopy class="h-6 w-6 duration-75 group-active:scale-90" />
	</button>
</div>
