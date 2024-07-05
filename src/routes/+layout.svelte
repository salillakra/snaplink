<script>
	import '../app.css';
	import { Button, DarkMode, } from 'flowbite-svelte';
</script>

<a href="/" class="flex justify-between m-2">
	<div class="flex justify-center items-center space-x-2">
		<img src="/logo.png" alt="logo" class="h-10 object-contain w-10" />
		<span class="text-dark text-3xl text-bold dark:text-white">SnapLink</span>
	</div>

	<div class="flex justify-center space-x-2">
		<Button color="blue">Sign Up</Button>
		<Button color="red">Logout</Button>
		<DarkMode />
	</div>
</a>

<slot />
