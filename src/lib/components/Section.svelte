<script lang="ts">
	import type { Snippet } from 'svelte';

	interface Props {
		color?: 'white' | 'gray';
		children: Snippet;
	}

	let { color = 'white', children }: Props = $props();

	const bgClasses = {
		white: 'bg-white',
		gray: 'bg-neutral-50'
	};
</script>

<section class="{bgClasses[color]} py-16 md:py-24">
	<div class="max-w-[800px] mx-auto px-6 md:px-8">
		{@render children()}
	</div>
</section>
