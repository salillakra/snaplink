<script lang="ts">
	import { DarkMode } from 'flowbite-svelte';
</script>

<DarkMode class="absolute right-2 top-2 z-10" />
<div class="h-screen bg-white text-gray-600 antialiased dark:bg-gray-900 dark:text-gray-400">
	<div id="svelte" class="relative max-h-screen w-full overflow-auto">
		<main class="bg-gray-50 dark:bg-gray-900">
			<div
				class="pt:mt-0 mx-auto flex flex-col items-center justify-center px-6 pt-8 dark:bg-gray-900 md:h-screen"
			>
				<div class="block md:max-w-lg">
					<img
						src="https://flowbite-admin-dashboard.vercel.app/images/illustrations/404.svg"
						alt="astronaut"
					/>
				</div>
				<div class="text-center xl:max-w-4xl">
					<h1
						class="mb-3 text-2xl font-bold leading-tight text-gray-900 dark:text-white sm:text-4xl lg:text-5xl"
					>
						Page not found
					</h1>
					<p
						class="mb-5 whitespace-normal text-left text-base font-normal text-gray-500 dark:text-gray-400 md:text-lg"
					>
						Oops! Looks like you followed a bad link. If you think this is a problem with us, please
						tell us.
					</p>
					<a
						href="/"
						class="inline-flex items-center justify-center rounded-lg bg-primary-700 px-5 py-2.5 text-center text-sm font-medium text-white focus-within:outline-none focus-within:ring-4 focus-within:ring-primary-300 hover:bg-primary-800 dark:bg-primary-600 dark:focus-within:ring-primary-800 dark:hover:bg-primary-700"
						role="button"
						><svg
							class="-ml-1 mr-2 h-5 w-5"
							fill="currentColor"
							viewBox="0 0 20 20"
							xmlns="http://www.w3.org/2000/svg"
							><path
								fill-rule="evenodd"
								d="M12.707 5.293a1 1 0 010 1.414L9.414 10l3.293 3.293a1 1 0 01-1.414 1.414l-4-4a1 1 0 010-1.414l4-4a1 1 0 011.414 0z"
								clip-rule="evenodd"
							></path></svg
						> Go back home</a
					>
				</div>
			</div>
		</main>
		<aside class="fixed bottom-5 right-5 z-50 hidden sm:block" data-svelte-h="svelte-17cyf0i">
			<div id="carbon-container"></div>
		</aside>
		<div
			id="svelte-announcer"
			aria-live="assertive"
			aria-atomic="true"
			style="position: absolute; left: 0px; top: 0px; clip: rect(0px, 0px, 0px, 0px); clip-path: inset(50%); overflow: hidden; white-space: nowrap; width: 1px; height: 1px;"
		>
			Flowbite Svelte Admin Dashboard - 404 page
		</div>
	</div>
</div>
