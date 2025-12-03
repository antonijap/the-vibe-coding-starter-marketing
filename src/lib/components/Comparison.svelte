<script lang="ts">
	import ComparisonCard from './ComparisonCard.svelte';
	import ComparisonListItem from './ComparisonListItem.svelte';
	import CodeInline from './CodeInline.svelte';
</script>

<section class="bg-white pb-16 md:pb-24">
	<div class="max-w-[800px] mx-auto px-6 md:px-8">
		<div class="relative">
			<div class="grid md:grid-cols-2 gap-4 md:gap-6 items-stretch">
			<!-- Without column -->
			<ComparisonCard>
				<ComparisonListItem type="error">
					Spend hours configuring Tailwind, ESLint, Prettier, TypeScript
				</ComparisonListItem>
				
				<ComparisonListItem type="error">
					☝️ You have no idea what this means
				</ComparisonListItem>
				
				<ComparisonListItem type="error">
					AI generates inconsistent, messy code every time
				</ComparisonListItem>
				
				<ComparisonListItem type="error">
					No design system, every component looks different
				</ComparisonListItem>
				
				<ComparisonListItem type="error">
					Burn tokens asking AI to fix its own config mistakes
				</ComparisonListItem>
				
				<ComparisonListItem type="error">
					Ship something that screams "AI made this"
				</ComparisonListItem>
			</ComparisonCard>

			<!-- With column -->
			<ComparisonCard hasMascot={true}>
				<ComparisonListItem type="success">
					Start building today
				</ComparisonListItem>
				
				<ComparisonListItem type="success">
					AI writes organized code
				</ComparisonListItem>
				
				<ComparisonListItem type="success">
					Looks professionally designed
				</ComparisonListItem>
				
				<ComparisonListItem type="success">
					Ship real products
				</ComparisonListItem>
				
				<img src="/mascot_pointing.png" alt="Mascot pointing" class="absolute bottom-0 right-0 w-48 md:w-72 lg:w-80 h-auto object-contain object-bottom" />
			</ComparisonCard>
			</div>
		</div>
	</div>
</section>
