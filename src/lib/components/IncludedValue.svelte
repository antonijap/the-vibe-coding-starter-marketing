<script lang="ts">
	import Card from './Card.svelte';
	import SectionHeader from './SectionHeader.svelte';
	import Section from './Section.svelte';
	import CodeInline from './CodeInline.svelte';
	import { DISCORD_LINK } from '$lib/constants';
</script>

<Section>
	<SectionHeader>
		A senior developer's foundation. One-time payment, instant download.
	</SectionHeader>

	<div class="grid grid-cols-2 gap-4">
		<Card color="blue" title="20+ hours of setup: done">
			<p>
				SvelteKit, Tailwind, TypeScript, ESLint, Prettier, testing, all configured. Run <code class="bg-neutral-200 px-1.5 py-0.5 rounded font-mono whitespace-nowrap">npm install</code>, start prompting.
			</p>
		</Card>

		<Card color="orange" title="Code guardrails">
			<p>
				AI writes messy code. Our guardrails auto-clean it. Consistent naming, proper structure, maintainable output. Every time.
			</p>
		</Card>

		<Card color="violet" title="Design system in Storybook">
			<p>
				11+ components, designed by a designer. Accessible, beautiful, documented. Your AI can see them, use them, extend them.
			</p>
		</Card>

		<Card color="cyan" title="You're not alone">
			<p>
				Join <a href={DISCORD_LINK} target="_blank" rel="noopener noreferrer" class="text-cyan-600 underline hover:text-cyan-900">The Vibe-Code Academy</a> Discord. Get help, share wins, learn advanced workflows from other vibe coders.
			</p>
		</Card>
	</div>
</Section>
