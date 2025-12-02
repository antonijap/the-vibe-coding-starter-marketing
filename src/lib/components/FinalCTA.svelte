<script lang="ts">
	import Button from './Button.svelte';
	import Section from './Section.svelte';
	import Footer from './Footer.svelte';
	import { CTA_LINK } from '$lib/constants';
</script>

<Section>
	<div class="text-center max-w-full mx-auto px-4 overflow-hidden">
		<div class="mb-4">
			<h1 class="font-['Bebas_Neue'] text-5xl sm:text-6xl md:text-7xl lg:text-8xl xl:text-9xl uppercase tracking-normal text-neutral-900 leading-[0.95]">
				<span class="block">You've read enough.</span>
				<span class="block text-neutral-400">Time to ship.</span>
			</h1>
		</div>

		<p class="text-neutral-600 mb-6 text-lg">
			You know the problem. Here's the fix. €49.99. Ship tomorrow.
		</p>

		<Button href={CTA_LINK} label="Get The Vibe-Coding Starter" />
	</div>
</Section>

<Footer />
