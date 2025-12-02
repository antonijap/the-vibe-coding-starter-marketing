<script lang="ts">
	import { DISCORD_LINK } from '$lib/constants';
</script>

<footer class="bg-neutral-50 py-8 md:py-12">
	<div class="max-w-[800px] mx-auto px-6 md:px-8">
		<div class="flex flex-col sm:flex-row items-center justify-between gap-4 text-neutral-500">
			<p>
				Made by <a href="https://apek.me" target="_blank" rel="noopener noreferrer" class="text-neutral-900 hover:underline">Antonija Pek</a>
			</p>
			<a
				href={DISCORD_LINK}
				target="_blank"
				rel="noopener noreferrer"
				class="text-neutral-900 hover:underline"
			>
				Discord
			</a>
		</div>
	</div>
</footer>

