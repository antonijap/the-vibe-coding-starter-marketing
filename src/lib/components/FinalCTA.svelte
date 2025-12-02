<script lang="ts">
	import Button from './Button.svelte';
	import Section from './Section.svelte';
	import Footer from './Footer.svelte';
	import { CTA_LINK } from '$lib/constants';
</script>

<Section>
	<div class="text-left max-w-full mx-auto px-4">
		<div class="mb-2 md:mb-4">
			<h1 class="heading-xl">
				<span class="block">You've read enough.</span>
				<span class="block text-red-600">Time to ship.</span>
			</h1>
		</div>

		<p class="text-neutral-600 text-lg md:text-xl mb-6 leading-relaxed">
			You know the problem. Here's the fix. €49.99. Ship tomorrow.
		</p>

		<Button href={CTA_LINK} label="Get The Vibe-Coding Starter" />
	</div>
</Section>

<Footer />
