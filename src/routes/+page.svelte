<script>
	import { onMount } from 'svelte';
	import { DarkMode } from 'flowbite-svelte';

	onMount(() => {
		// Add your initialization code here
	});
</script>

<div class="place-items-end px-4 grid">
	<DarkMode />
</div>

<main class="flex min-h-[90vh] items-center justify-center bg-gray-400 dark:bg-gray-900">
	<div class="rounded bg-white px-8 py-6 shadow-md dark:bg-gray-800">
		<h1 class="mb-4 text-2xl font-bold dark:text-white">Under Construction</h1>
		<p class="mb-4 text-gray-700 dark:text-gray-300">This page is currently under construction.</p>
		<a href="/dashboard" class="text-blue-500 hover:text-blue-700">Go to Dashboard</a>
	</div>
</main>

<style>
	/* Add your custom styles here */
</style>
