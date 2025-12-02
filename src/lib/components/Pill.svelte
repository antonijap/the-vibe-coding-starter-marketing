<script lang="ts">
	import type { Snippet } from 'svelte';

	interface Props {
		children: Snippet;
	}

	let { children }: Props = $props();
</script>

<span class="inline-flex items-center justify-center bg-white border-2 border-black rounded-full shadow-[0_4px_0_0_rgb(0,0,0)] overflow-hidden mx-1.5" style="height: 0.75em; width: 1em; vertical-align: middle;">
	{@render children()}
</span>

