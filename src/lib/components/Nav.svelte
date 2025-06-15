<script>
	import Heading from '$lib/components/Heading.svelte'
</script>

<aside class="flex flex-col bg-black/50">
	<Heading>
		<h1 class="text-2xl text-emerald-400">> useful snippets_</h1>
	</Heading>
	<nav>
		<ul class="flex flex-col gap-3">
			<li>
				<Heading>
					<a href="#category-1">category 1</a>
				</Heading>
			</li>
			<li class="px-3">
				<a href="#snippet-1">snippet 1</a>
			</li>
			<li class="px-3">
				<a href="#snippet-2">snippet 2</a>
			</li>
			<li>
				<Heading>
					<a href="#category-2">category 2</a>
				</Heading>
			</li>
			<li class="px-3">
				<a href="#snippet-3">snippet 3</a>
			</li>
		</ul>
	</nav>
	<button
		class="sticky top-0 cursor-pointer py-4 underline"
		onclick={() => window.scrollTo({ top: 0, behavior: 'smooth' })}
	>
		scroll to top
	</button>
</aside>
