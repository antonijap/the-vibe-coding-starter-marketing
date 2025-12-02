<script lang="ts">
	import type { Snippet } from 'svelte';

	interface Props {
		level?: 1 | 2;
		children: Snippet;
	}

	let { level = 2, children }: Props = $props();
</script>

{#if level === 1}
	<h1 class="heading-xl mb-6 md:mb-8">
		{@render children()}
	</h1>
{:else}
	<h2 class="heading-lg mb-4 md:mb-6">
		{@render children()}
	</h2>
{/if}

