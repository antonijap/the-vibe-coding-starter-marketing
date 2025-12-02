<script lang="ts">
	import type { Snippet } from 'svelte';

	interface Props {
		color: 'yellow' | 'pink' | 'green' | 'blue' | 'orange' | 'violet' | 'cyan' | 'purple';
		title?: string;
		children: Snippet;
	}

	let { color, title, children }: Props = $props();

	const colorClasses: Record<string, { bg: string; title: string; text: string }> = {
		yellow: { bg: 'bg-white', title: 'text-neutral-900', text: 'text-neutral-600' },
		pink: { bg: 'bg-white', title: 'text-neutral-900', text: 'text-neutral-600' },
		green: { bg: 'bg-white', title: 'text-neutral-900', text: 'text-neutral-600' },
		blue: { bg: 'bg-white', title: 'text-neutral-900', text: 'text-neutral-600' },
		orange: { bg: 'bg-white', title: 'text-neutral-900', text: 'text-neutral-600' },
		violet: { bg: 'bg-white', title: 'text-neutral-900', text: 'text-neutral-600' },
		cyan: { bg: 'bg-white', title: 'text-neutral-900', text: 'text-neutral-600' },
		purple: { bg: 'bg-purple-100', title: 'text-purple-900', text: 'text-purple-800' }
	};

	const classes = colorClasses[color];
</script>

<div class="{classes.bg} border-2 border-black rounded-2xl shadow-[0_8px_0_0_rgb(0,0,0)]">
	<div class="p-6 rounded-xl">
		{#if title}
			<h3 class="font-medium {classes.title} mb-2">{title}</h3>
		{/if}
		<div class="{classes.text}">
			{@render children()}
		</div>
	</div>
</div>
