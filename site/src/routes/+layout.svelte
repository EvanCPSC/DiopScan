<script lang="ts">
	import favicon from '#lib/assets/diopscan.svg';
	import type { LayoutProps } from './$types';

	let { children }: LayoutProps = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>DiopScan - Cancer Classifier</title>
</svelte:head>

{@render children()}
