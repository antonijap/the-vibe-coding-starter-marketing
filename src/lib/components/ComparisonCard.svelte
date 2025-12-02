<script lang="ts">
	import type { Snippet } from 'svelte';

	interface Props {
		children: Snippet;
	}

	let { children }: Props = $props();
</script>

<div class="bg-white border-2 border-black rounded-2xl shadow-[0_8px_0_0_rgb(0,0,0)] p-6 relative z-10 flex-1 flex flex-col">
	<ul class="space-y-4 flex-1">
		{@render children()}
	</ul>
</div>

