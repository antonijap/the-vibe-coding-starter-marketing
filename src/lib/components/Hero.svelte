<script lang="ts">
	import Heading from './Heading.svelte';
	import Pill from './Pill.svelte';
	import YouTubeEmbed from './YouTubeEmbed.svelte';
	import { YOUTUBE_VIDEO_ID } from '$lib/constants';
</script>

<section class="min-h-[60vh] md:min-h-[80vh] flex flex-col justify-center text-center">
	<div class="max-w-3xl mx-auto">
		<Heading level={1}>
			<span class="whitespace-nowrap">Your AI <Pill><img src="/mascot_smiling.png" alt="Smiling mascot" class="h-full w-auto object-cover" /></Pill> writes code.</span><br />
			<span class="text-neutral-400 whitespace-nowrap">Not good code.<Pill><img src="/mascot_thinking.png" alt="Thinking mascot" class="h-full w-auto object-cover" /></Pill></span>
		</Heading>

		<p class="text-neutral-600 text-base md:text-lg mb-10 md:mb-16 leading-relaxed mx-auto max-w-2xl">
			It works for one feature. Add a second and things start breaking. Add a third and you're rewriting everything. AI doesn't think about tomorrow. It solves today's prompt and leaves tomorrow's mess. <strong class="text-neutral-900">That's not scalable. That's a dead end.</strong>
		</p>

		<YouTubeEmbed videoId={YOUTUBE_VIDEO_ID} title="The Vibe-Coding Starter Kit" />
	</div>
</section>
