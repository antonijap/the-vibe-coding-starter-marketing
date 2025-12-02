<script lang="ts">
	import Hero from '$lib/components/Hero.svelte';
	import Comparison from '$lib/components/Comparison.svelte';
	import AlmostDone from '$lib/components/AlmostDone.svelte';
	import ValuePillars from '$lib/components/ValuePillars.svelte';
	import FinalCTA from '$lib/components/FinalCTA.svelte';
</script>

<main class="min-h-screen bg-white">
	<div class="max-w-[800px] mx-auto py-12 md:py-20 px-6 md:px-8">
		<Hero />
	</div>
	<AlmostDone />
	<Comparison />
	<ValuePillars />
	<FinalCTA />
</main>
