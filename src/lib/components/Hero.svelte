<script lang="ts">
	import Heading from './Heading.svelte';
	import Pill from './Pill.svelte';
	import YouTubeEmbed from './YouTubeEmbed.svelte';
	import { YOUTUBE_VIDEO_ID } from '$lib/constants';
</script>

<section class="pt-16 md:pt-24 text-left">
	<div>
		<Heading level={1}>
			<span class="text-neutral-900">You let <Pill><img src="/mascot_smiling.png" alt="Smiling mascot" class="h-full w-auto object-cover" /></Pill> AI decide everything.</span><br />
			<span class="text-red-600">Bad idea. <Pill><img src="/mascot_thinking.png" alt="Thinking mascot" class="h-full w-auto object-cover" /></Pill></span>
		</Heading>

		<p class="text-neutral-900 text-lg md:text-xl lg:text-2xl mb-10 md:mb-16 leading-relaxed">
			<strong>Tech stack. Structure. Architecture.</strong> AI picks easy, not scalable. We made those decisions right. You build on solid ground.
		</p>

		<YouTubeEmbed videoId={YOUTUBE_VIDEO_ID} title="The Vibe-Coding Starter Kit" />
	</div>
</section>
