<script lang="ts">
	import type { Snippet } from 'svelte';
	import ComparisonIcon from './ComparisonIcon.svelte';

	interface Props {
		type: 'success' | 'error';
		children: Snippet;
	}

	let { type, children }: Props = $props();
</script>

<li class="flex items-start gap-3">
	<ComparisonIcon {type} />
	<span class="text-neutral-600">{@render children()}</span>
</li>

