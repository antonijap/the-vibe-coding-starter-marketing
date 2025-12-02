<script lang="ts">
	interface Props {
		href: string;
		label: string;
		price?: string;
	}

	let { href, label, price }: Props = $props();
</script>

<a
	{href}
	target="_blank"
	rel="noopener noreferrer"
	class="button group inline-flex items-center gap-3 text-white px-8 py-4 text-lg rounded-2xl bg-black relative transition-transform hover:scale-105"
>
	<span class="font-medium relative z-10">{label}</span>
	
	{#if price}
		<span class="text-neutral-400 relative z-10">{price}</span>
	{/if}
</a>

<style>
	.button {
		overflow: visible;
	}
</style>
