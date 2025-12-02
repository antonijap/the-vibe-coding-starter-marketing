<script lang="ts">
	interface Props {
		videoId: string;
		title?: string;
	}

	let { videoId, title = 'Video' }: Props = $props();
</script>

<div class="-mx-6 md:-mx-8 lg:-mx-12 max-w-[990px] md:max-w-[1100px] lg:max-w-[1210px] mx-auto">
	<iframe
		class="w-full aspect-video rounded-lg"
		src="https://www.youtube.com/embed/{videoId}"
		{title}
		frameborder="0"
		allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
		allowfullscreen
	></iframe>
</div>

