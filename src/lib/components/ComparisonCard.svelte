<script lang="ts">
	import type { Snippet } from 'svelte';

	interface Props {
		children: Snippet;
		hasMascot?: boolean;
	}

	let { children, hasMascot = false }: Props = $props();
</script>

<div class="bg-white border-2 border-black rounded-2xl shadow-[0_8px_0_0_rgb(0,0,0)] p-6 {hasMascot ? 'pb-32 md:pb-6' : ''} relative z-10 flex-1 flex flex-col">
	<ul class="space-y-4 flex-1">
		{@render children()}
	</ul>
</div>

