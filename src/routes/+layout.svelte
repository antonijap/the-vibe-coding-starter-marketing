<script>
	import '../app.css';

	let { children } = $props();
</script>

<svelte:head>
	<title>The Vibe-Code Starter Kit | From Idea to First Prompt in Under 5 Minutes</title>
	<meta
		name="description"
		content="The design-first foundation for Vibe Coders. Skip setup, enforce quality, and launch in minutes. Stop wasting AI tokens on configuration."
	/>
</svelte:head>

{@render children()}

