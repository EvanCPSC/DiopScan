<script lang="ts">
	import favicon from '#lib/assets/diopscan.svg';
	import type { LayoutProps } from './$types';

	let { children }: LayoutProps = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>DiopScan - Cancer Classifier</title>
	<link rel="preconnect" href="https://fonts.googleapis.com">
	<link rel="preconnect" href="https://fonts.gstatic.com">
	<link href="https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap" rel="stylesheet">
	<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0&icon_names=search" />
</svelte:head>

{@render children()}

<style>
	:global(:root) {
		--diop-light: #3dc4b6;
		--diop-dark: #158478;
		--primary-bg: #f5f5f5;
		--text-color: #333333;
		--shadow-color: rgba(0, 0, 0, 0.1);
	}
	:global(body) {
		margin: 0;
		font-family: "Open Sans", sans-serif;
		background-color: var(--primary-bg);
		color: var(--text-color);
	}
	:global(nav) {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 1rem 2rem;
		background-color: white;
		box-shadow: 0 2px 4px var(--shadow-color);
		margin: auto;
	}
	:global(nav img) {
		width: 30px;
	}
	:global(.nav-left) {
		display: flex;
		align-items: center;
		font-size: 1.4rem;
		font-weight: bold;
		color: var(--diop-dark);
		gap: 0.5rem;
	}
	:global(.nav-right) {
		display: flex;
		gap: 2rem;
	}
	:global(.nav-link) {
		text-decoration: none;
		color: var(--font-color);
		border-bottom: 3px solid transparent;
	}
	:global(.nav-link:hover) {
		border-bottom: 3px solid var(--diop-light);
		color: var(--diop-dark);
	}
</style>