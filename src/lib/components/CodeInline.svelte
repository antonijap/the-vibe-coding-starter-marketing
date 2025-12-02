<script lang="ts">
	import type { Snippet } from 'svelte';

	interface Props {
		bgColor?: string;
		children: Snippet;
	}

	let { bgColor = 'bg-neutral-100', children }: Props = $props();
</script>

<code class="{bgColor} px-1.5 py-0.5 rounded font-mono">{@render children()}</code>
