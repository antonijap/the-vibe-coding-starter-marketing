<script lang="ts">
	import Card from './Card.svelte';

	interface Props {
		videoId: string;
		title?: string;
	}

	let { videoId, title = 'Video' }: Props = $props();
</script>

<Card color="purple">
	<div class="p-0 -m-4">
		<iframe
			class="w-full aspect-video rounded-xl"
			src="https://www.youtube.com/embed/{videoId}"
			{title}
			frameborder="0"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
			allowfullscreen
		></iframe>
	</div>
</Card>

