<script lang="ts">
	import type { Snippet } from 'svelte';

	interface Props {
		variant?: 'filled' | 'outlined';
		size?: 'sm' | 'md' | 'lg';
		children: Snippet;
	}

	let { variant = 'filled', size = 'md', children }: Props = $props();

	const sizeClasses = {
		sm: 'w-10 h-10',
		md: 'w-14 h-14',
		lg: 'w-16 h-16'
	};

	const iconSizeClasses = {
		sm: '[&>svg]:w-5 [&>svg]:h-5',
		md: '[&>svg]:w-7 [&>svg]:h-7',
		lg: '[&>svg]:w-8 [&>svg]:h-8'
	};
</script>

<div
	class="flex items-center justify-center rounded-full {sizeClasses[size]} {iconSizeClasses[size]} {variant === 'filled'
		? 'bg-orange-600 text-white'
		: 'bg-orange-100 text-orange-600 border-2 border-orange-600'}"
>
	{@render children()}
</div>

