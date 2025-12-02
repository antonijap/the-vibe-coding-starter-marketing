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
			<ComparisonCard>
				<ComparisonListItem type="success">
					Run <CodeInline>npm install</CodeInline> and start building
				</ComparisonListItem>
				
				<ComparisonListItem type="success">
					Guardrails auto-format and clean AI output
				</ComparisonListItem>
				
				<ComparisonListItem type="success">
					11+ components in Storybook, designed by a designer
				</ComparisonListItem>
				
				<ComparisonListItem type="success">
					Every token goes into features, not setup
				</ComparisonListItem>
				
				<ComparisonListItem type="success">
					Ship something that looks professionally designed
				</ComparisonListItem>
			</ComparisonCard>
			</div>
		</div>
	</div>
</section>
