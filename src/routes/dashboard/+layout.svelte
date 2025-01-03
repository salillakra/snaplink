<script>
	import {
		SidebarDropdownItem,
		SidebarDropdownWrapper,
		Navbar,
		NavBrand,
		NavLi,
		NavUl,
		NavHamburger,
		Avatar,
		Dropdown,
		DropdownItem,
		DropdownHeader,
	} from 'flowbite-svelte';
	import Sidebar from '../components/Sidebar.svelte';
</script>

<Navbar
	class="bg-gradient-to-r from-green-100 to-gray-200 dark:bg-gradient-to-r dark:from-black dark:to-zinc-950"
>

	<NavBrand href="/">
		<img src="/kitty_logo.png" class="me-3 h-6 sm:h-9" alt="snaplink Logo" />
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">SnapLink</span
		>
	</NavBrand>

	<div class="flex items-center md:order-2">
		<Avatar
			id="avatar-menu"
			src="https://img.fixthephoto.com/blog/images/gallery/news_preview_mob_image__preview_11368.png"
		/>
		<NavHamburger class1="w-full md:flex md:w-auto md:order-1" />
	</div>
	<Dropdown placement="bottom" triggeredBy="#avatar-menu">
		<DropdownHeader>
			<span class="block text-sm">Bonnie Green</span>
			<span class="block truncate text-sm font-medium">name@flowbite.com</span>
		</DropdownHeader>
		<DropdownItem>Sign out</DropdownItem>
	</Dropdown>
	<NavUl>
		<NavLi class="lato-bold" href="/dashboard/about">About</NavLi>
		<NavLi class="lato-bold" href="/dashboard/pricing">Pricing</NavLi>
		<NavLi class="lato-bold" href="/dashboard/contact">Contact</NavLi>
		<SidebarDropdownWrapper class="sm:hidden" label="Dashboard">
			<svelte:fragment slot="icon">
				<img src="/dashboard.png" alt="dashboard" class="h-5 w-5" />
			</svelte:fragment>
			<SidebarDropdownItem href="statistics" label="Statistics" />
			<SidebarDropdownItem href="create-link" label="Create link" />
			<SidebarDropdownItem href="links" label="My links" />
			<SidebarDropdownItem href="settings" label="Settings" />
			
		</SidebarDropdownWrapper>
	</NavUl>
</Navbar>

<div class="flex">
	<Sidebar />
	<slot />
</div>
