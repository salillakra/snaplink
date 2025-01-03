<script>
	import { P, DropdownDivider, DarkMode } from 'flowbite-svelte';

	const menu_items = {
		statistics: {
			name: 'Statistics',
			link: '/dashboard/statistics',
			icon: 'analytics'
		},
		create_link: {
			name: 'Create link',
			link: '/dashboard/create-link',
			icon: 'add_circle'
		},
		my_links: {
			name: 'My links',
			link: '/dashboard/links',
			icon: 'link'
		},
		settings: {
			name: 'Settings',
			link: '/dashboard/settings',
			icon: 'settings'
		}
	};
</script>

<div
	class="relative hidden h-[92vh] w-[20%] min-w-44 border-r-2 border-gray-950 bg-white dark:bg-black sm:block"
>
	<div
		class=" flex cursor-pointer items-center space-x-3 pl-2 hover:animate-pulse dark:text-white lg:pl-5"
	>
		<span class="material-symbols-outlined"> dashboard </span>
		<span class="lato-bold my-6 text-lg lg:text-2xl">Dashboard</span>
	</div>
	<DropdownDivider class="bg-black dark:bg-white" />
	<div class=" mt-4 flex flex-col items-center justify-center space-y-1">
		{#each Object.entries(menu_items) as [key, value]}
			<a
				href={value.link}
				id={key}
				class="text-md dark:text lato-regular flex h-12 w-full items-center gap-3 rounded-lg px-2 transition-all hover:bg-slate-600 hover:text-white dark:text-gray-300 dark:hover:bg-slate-500 dark:hover:text-white lg:w-11/12 lg:gap-4 lg:pl-2 lg:text-xl"
			>
				<span class="material-symbols-outlined">{value.icon}</span>
				{value.name}</a
			>
		{/each}

		<DarkMode class="absolute bottom-8 left-4" />
	</div>
</div>
