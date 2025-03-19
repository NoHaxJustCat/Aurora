<script lang="ts">
	import { page } from '$app/state';
</script>

<main class="container mx-auto">
	<h1 class="text-center text-9xl font-bold text-neutral-100">{page.status}</h1>
	<h2 class="mt-8 text-center text-6xl font-medium text-neutral-100">{page.error?.message}</h2>
	<p class="mt-4 text-center text-lg text-neutral-200">
		{#if page.status === 404}
			The page you are looking for does not exist.
		{:else}
			An error occurred.
		{/if}
	</p>
</main>
