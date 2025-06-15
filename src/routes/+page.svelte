<script>
	import Category from '$lib/components/Category.svelte'
	import Code from '$lib/components/Code.svelte'
	import Description from '$lib/components/Description.svelte'
	import Heading from '$lib/components/Heading.svelte'
	import Nav from '$lib/components/Nav.svelte'
	import Snippet from '$lib/components/Snippet.svelte'
</script>

<Nav />

<div class="grow">
	<main>
		<Category title="category 1" />
		<Snippet title="snippet 1">
			<Description>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
				incididunt ut labore et dolore magnam aliquam quaerat voluptatem.
			</Description>
			<Code
				code={`
const x = 1;
const y = 2;
`}
			/>
		</Snippet>
		<Snippet title="snippet 1">
			<Description>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
				incididunt ut labore et dolore magnam aliquam quaerat voluptatem.
			</Description>
			<Description>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
				incididunt ut labore et dolore magnam aliquam quaerat voluptatem.
			</Description>
			<Code
				code={`
const x = 1;
const y = 2;
`}
			/>
		</Snippet>

		<Category title="category 1" />
		<Snippet title="snippet 1">
			<Description>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
				incididunt ut labore et dolore magnam aliquam quaerat voluptatem.
			</Description>
			<Code
				code={`
const x = 1;
const y = 2;
`}
			/>
		</Snippet>
		<Snippet title="snippet 1">
			<Description>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
				incididunt ut labore et dolore magnam aliquam quaerat voluptatem.
			</Description>
			<Description>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
				incididunt ut labore et dolore magnam aliquam quaerat voluptatem.
			</Description>
			<Code
				code={`
const x = 1;
const y = 2;
`}
			/>
		</Snippet>

		<Category title="category 1" />
		<Snippet title="snippet 1">
			<Description>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
				incididunt ut labore et dolore magnam aliquam quaerat voluptatem.
			</Description>
			<Code
				code={`
const x = 1;
const y = 2;
`}
			/>
		</Snippet>
		<Snippet title="snippet 1">
			<Description>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
				incididunt ut labore et dolore magnam aliquam quaerat voluptatem.
			</Description>
			<Description>
				Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
				incididunt ut labore et dolore magnam aliquam quaerat voluptatem.
			</Description>
			<Code
				code={`
const x = 1;
const y = 2;
`}
			/>
		</Snippet>
	</main>

	<footer
		class="flex flex-col justify-evenly gap-3 px-3 py-6 text-center md:flex-row md:items-center md:gap-6"
	>
		<span>
			Developed by
			<a href="https://dannyharris.dev" class="text-emerald-400 underline">dannyharris.dev</a>
		</span>
		<span>Copyright © 2023–{new Date().getFullYear()} Danny Harris</span>
		<span>
			Get your own website at
			<a href="https://freelancewebdev.dev" class="text-emerald-400 underline">
				freelancewebdev.dev
			</a>
		</span>
	</footer>
</div>
