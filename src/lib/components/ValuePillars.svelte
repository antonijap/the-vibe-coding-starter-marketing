<script lang="ts">
	import { DISCORD_LINK } from '$lib/constants';
</script>

<section class="py-16 md:py-24 relative overflow-hidden" style="background-color: #FCFBFC;">
	<div class="max-w-[800px] mx-auto px-6 md:px-8 relative z-10">
		<div class="text-center md:text-left w-full md:max-w-sm">
			<h2 class="font-['Bebas_Neue'] text-5xl sm:text-6xl md:text-7xl lg:text-8xl xl:text-9xl uppercase tracking-normal text-neutral-900 leading-[0.95] mb-4 md:mb-12">
				You're not alone
			</h2>

			<p class="text-base leading-relaxed mb-6">
				Get help when you're stuck. Share your wins. Learn advanced workflows from other vibe coders building real products.
			</p>

			<a
				href={DISCORD_LINK}
				target="_blank"
				rel="noopener noreferrer"
				class="inline-flex items-center gap-3 text-white px-8 py-4 text-lg rounded-2xl bg-[#5865F2] hover:bg-[#4752C4] transition-colors font-medium md:inline-flex"
			>
				<svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor">
					<path d="M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515a.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0a12.64 12.64 0 0 0-.617-1.25a.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057a.082.082 0 0 0 .031.057a19.9 19.9 0 0 0 5.993 3.03a.078.078 0 0 0 .084-.028a14.09 14.09 0 0 0 1.226-1.994a.076.076 0 0 0-.041-.106a13.107 13.107 0 0 1-1.872-.892a.077.077 0 0 1-.008-.128a10.2 10.2 0 0 0 .372-.292a.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127a12.299 12.299 0 0 1-1.873.892a.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028a19.839 19.839 0 0 0 6.002-3.03a.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03zM8.02 15.33c-1.183 0-2.157-1.085-2.157-2.419c0-1.333.956-2.419 2.157-2.419c1.21 0 2.176 1.096 2.157 2.42c0 1.333-.956 2.418-2.157 2.418zm7.975 0c-1.183 0-2.157-1.085-2.157-2.419c0-1.333.955-2.419 2.157-2.419c1.21 0 2.176 1.096 2.157 2.42c0 1.333-.946 2.418-2.157 2.418z"/>
				</svg>
				Join Discord
			</a>
		</div>
	</div>
	<img src="/mascot_happy.png" alt="Happy mascot" class="absolute -right-60 md:-right-80 lg:-right-96 top-[60%] md:top-[65%] -translate-y-1/2 -rotate-12 w-[600px] md:w-[900px] lg:w-[1200px] z-0 hidden md:block" />
</section>
