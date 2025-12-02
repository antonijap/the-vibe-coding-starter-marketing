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
	class="button group inline-flex items-center gap-3 text-white px-8 py-4 text-lg rounded-2xl bg-black relative"
>
	<span class="font-medium relative z-10">{label}</span>
	
	{#if price}
		<span class="text-neutral-400 relative z-10">{price}</span>
	{/if}
</a>

<style>
	.button {
		overflow: visible;
		transform-origin: center;
		transition: transform 0.3s ease-out;
	}
	
	.button:hover {
		animation: continuousGrow 120s ease-out forwards;
	}
	
	.button:not(:hover) {
		animation: none;
		transform: scale(1);
	}
	
	@keyframes continuousGrow {
		0% {
			transform: scale(1);
		}
		100% {
			transform: scale(10);
		}
	}
</style>
