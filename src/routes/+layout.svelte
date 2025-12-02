<script>
	import '../app.css';

	let { children } = $props();

	// SEO Configuration
	const seo = {
		title: "The Vibe-Coding Starter Kit | AI Code Foundation for Non-Developers",
		description: "Stop wasting time on setup. Your AI writes better code with our professional foundation. Start building today, ship real products. €49.99",
		url: "https://the-vibe-coding-starter.com",
		image: "https://the-vibe-coding-starter.com/og-image.png",
		keywords: "AI coding, cursor AI, no-code alternative, SvelteKit starter, AI development kit, non-technical founder, vibe coding, AI code generator, side project starter, quick launch"
	};
</script>

<svelte:head>
	<!-- Primary Meta Tags -->
	<title>{seo.title}</title>
	<meta name="title" content={seo.title} />
	<meta name="description" content={seo.description} />
	<meta name="keywords" content={seo.keywords} />
	<meta name="author" content="The Vibe-Coding Starter" />
	<meta name="robots" content="index, follow" />
	<link rel="canonical" href={seo.url} />

	<!-- Open Graph / Facebook -->
	<meta property="og:type" content="website" />
	<meta property="og:url" content={seo.url} />
	<meta property="og:title" content={seo.title} />
	<meta property="og:description" content={seo.description} />
	<meta property="og:image" content={seo.image} />
	<meta property="og:site_name" content="The Vibe-Coding Starter Kit" />
	<meta property="og:locale" content="en_US" />

	<!-- Twitter -->
	<meta property="twitter:card" content="summary_large_image" />
	<meta property="twitter:url" content={seo.url} />
	<meta property="twitter:title" content={seo.title} />
	<meta property="twitter:description" content={seo.description} />
	<meta property="twitter:image" content={seo.image} />

	<!-- Additional SEO -->
	<meta name="theme-color" content="#ffffff" />
	<meta name="apple-mobile-web-app-capable" content="yes" />
	<meta name="apple-mobile-web-app-status-bar-style" content="default" />
	<meta name="format-detection" content="telephone=no" />

	<!-- Structured Data / JSON-LD for Google -->
	<script type="application/ld+json">
		{JSON.stringify({
			"@context": "https://schema.org",
			"@type": "Product",
			"name": "The Vibe-Coding Starter Kit",
			"description": "Professional SvelteKit foundation that makes your AI write better code. Start building today, ship real products.",
			"image": seo.image,
			"brand": {
				"@type": "Brand",
				"name": "The Vibe-Coding Starter"
			},
			"offers": {
				"@type": "Offer",
				"price": "49.99",
				"priceCurrency": "EUR",
				"availability": "https://schema.org/InStock",
				"url": "https://antonija.lemonsqueezy.com/buy/2355a849-0f60-443c-a2a7-4d5a74bd4fe3"
			},
			"aggregateRating": {
				"@type": "AggregateRating",
				"ratingValue": "5",
				"reviewCount": "1"
			}
		})}
	</script>

	<script type="application/ld+json">
		{JSON.stringify({
			"@context": "https://schema.org",
			"@type": "SoftwareApplication",
			"name": "The Vibe-Coding Starter Kit",
			"applicationCategory": "DeveloperApplication",
			"operatingSystem": "Cross-platform",
			"offers": {
				"@type": "Offer",
				"price": "49.99",
				"priceCurrency": "EUR"
			},
			"description": "AI-powered development starter kit for non-technical founders and designers"
		})}
	</script>
</svelte:head>

{@render children()}

