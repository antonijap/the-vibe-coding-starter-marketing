<script lang="ts">
	interface Props {
		type: 'success' | 'error';
	}

	let { type }: Props = $props();
	
	const bgColor = type === 'success' ? 'bg-green-100' : 'bg-red-100';
	const iconColor = type === 'success' ? 'text-green-600' : 'text-red-500';
</script>

<span class="w-6 h-6 {bgColor} rounded-full flex items-center justify-center shrink-0 mt-0.5">
	{#if type === 'success'}
		<svg class="w-3.5 h-3.5 {iconColor}" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2.5">
			<path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
		</svg>
	{:else}
		<svg class="w-3.5 h-3.5 {iconColor}" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2.5">
			<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
		</svg>
	{/if}
</span>

