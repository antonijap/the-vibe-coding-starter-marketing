<script lang="ts">
	import type { Snippet } from 'svelte';
	import Heading from './Heading.svelte';

	interface Props {
		children: Snippet;
	}

	let { children }: Props = $props();
</script>

<div class="mb-12">
	<Heading>
		{@render children()}
	</Heading>
</div>

