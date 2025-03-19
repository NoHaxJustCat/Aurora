<script lang="ts">
	import { base } from '$app/paths';
	import Navbar from '$lib/components/layout/Navbar.svelte';
	import '$lib/styles/app.css';

	let { children } = $props();
</script>

<Navbar />

<div class="filter-blur-xl min-h-screen w-full py-16 xl:py-24">
	<div class="fixed top-0 right-0 bottom-0 left-0 z-[-1] backdrop-blur-2xl backdrop-filter"></div>
	<!-- style="background: url({base}/background.jpg) no-repeat center center; background-size: cover;" -->

	<div class="relative container mx-auto flex px-4 sm:px-6">
		<main class="container w-screen flex-shrink-0 flex-grow px-0 xl:px-4">
			<div class="main-container searchable-content box-content">
				{@render children?.()}
			</div>
			<!-- <Footer /> -->
		</main>
	</div>
</div>
