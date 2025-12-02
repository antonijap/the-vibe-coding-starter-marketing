<script lang="ts">
	import type { Snippet } from 'svelte';

	interface Props {
		level?: 1 | 2;
		children: Snippet;
	}

	let { level = 2, children }: Props = $props();
</script>

{#if level === 1}
	<h1 class="font-['Bebas_Neue'] text-5xl sm:text-6xl md:text-7xl lg:text-8xl uppercase tracking-normal text-neutral-900 leading-[0.95] mb-6 md:mb-8">
		{@render children()}
	</h1>
{:else}
	<h2 class="font-['Bebas_Neue'] text-3xl sm:text-4xl md:text-5xl lg:text-6xl uppercase tracking-normal text-neutral-900 leading-[0.95] mb-4 md:mb-6">
		{@render children()}
	</h2>
{/if}

