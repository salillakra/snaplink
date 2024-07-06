<script>
	import { P, DropdownDivider } from 'flowbite-svelte';

	const menu_items = {
		statistics: {
			name: 'statistics',
			link: 'statistics',
			icon: 'analytics'
		},
		create_link: {
			name: 'Create link',
			link: 'create-link',
			icon: 'add_circle'
		},
		my_links: {
			name: 'My links',
			link: 'links',
			icon: 'link'
		},
		settings: {
			name: 'Settings',
			link: 'settings',
			icon: 'settings'
		}
	};
</script>

<div class="hidden h-[92vh] w-[20%] border-r-2 border-gray-950 bg-white dark:bg-black sm:block">
	<div class="flex cursor-pointer items-center space-x-3 pl-6 hover:animate-pulse">
		<span class="material-symbols-outlined text-black dark:text-white"> dashboard </span>
		<P size="3xl" class="my-5" weight="medium">Dashboard</P>
	</div>
	<DropdownDivider class="bg-black dark:bg-white" />
	<div class=" flex w-full flex-col items-center justify-center space-y-1 p-2">
		{#each Object.entries(menu_items) as [key, value]}
			<a
				href={value.link}
				id={key}
				class="flex h-12 w-11/12 items-center gap-5 rounded-md p-2 text-xl transition-all hover:bg-slate-600 hover:text-white dark:text-white dark:hover:bg-slate-500"
			>
				<span class="material-symbols-outlined">{value.icon}</span>
				{value.name}</a
			>
		{/each}
	</div>
</div>
