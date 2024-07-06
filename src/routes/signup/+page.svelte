<script>
	import { DarkMode } from 'flowbite-svelte';
</script>

<DarkMode class="absolute right-2 top-2 z-10" />

<div
	class="relative h-screen bg-gradient-to-br from-sky-50 to-gray-200 py-16 dark:from-slate-700 dark:to-slate-900"
>
	<div class="container relative m-auto px-6 text-gray-500 md:px-12 xl:px-40">
		<div class="m-auto md:w-8/12 lg:w-6/12 xl:w-6/12">
			<div class="rounded-xl bg-white shadow-xl dark:bg-black">
				<div class="p-6 sm:p-16">
					<div class="space-y-4">
						<img src="/kitty_logo.png" loading="lazy" class="w-10" alt="snaplink logo" />
						<h2 class="mb-8 text-2xl font-bold text-cyan-900 dark:text-orange-500">
							Sign in to unlock the <br /> best of Qlink.
						</h2>
					</div>
					<div class="mt-16 grid space-y-4">
						<button
							class="group h-12 rounded-full border-2 border-gray-300 px-6 transition duration-300
 hover:border-blue-400 focus:bg-blue-50 active:bg-blue-100"
						>
							<div class="relative flex items-center justify-center space-x-4">
								<img src="/google_logo.png" class="absolute left-0 w-5" alt="google logo" />
								<span
									class="block w-max text-sm font-semibold tracking-wide text-gray-700 transition duration-300 group-hover:text-blue-600 dark:text-white sm:text-base"
									>Continue with Google</span
								>
							</div>
						</button>
						<button
							class="group h-12 rounded-full border-2 border-gray-300 px-6 transition duration-300
 hover:border-blue-400 focus:bg-blue-50 active:bg-blue-100"
						>
							<div class="relative flex items-center justify-center space-x-4">
								<img src="/microsoft_logo.png" class="absolute left-0 w-5" alt="microsoft logo" />
								<span
									class="block w-max text-sm font-semibold tracking-wide text-gray-700 transition duration-300 group-hover:text-blue-600 dark:text-white sm:text-base"
									>Continue with Microsoft</span
								>
							</div>
						</button>
						<button
							class="group h-12 rounded-full border-2 border-gray-300 px-6 transition duration-300
                                     hover:border-blue-400 focus:bg-blue-50 active:bg-blue-100"
						>
							<div class="relative flex items-center justify-center space-x-4">
								<img
									src="https://upload.wikimedia.org/wikipedia/en/0/04/Facebook_f_logo_%282021%29.svg"
									class="absolute left-0 w-5"
									alt="Facebook logo"
								/>
								<span
									class="block w-max text-sm font-semibold tracking-wide text-gray-700 transition duration-300 group-hover:text-blue-600 dark:text-white sm:text-base"
									>Continue with Facebook</span
								>
							</div>
						</button>
					</div>

					<div class="mt-32 space-y-4 text-center text-gray-600 sm:-mb-8">
						<p class="text-xs dark:text-gray-300">
							By proceeding, you agree to our <a href="#" class="underline">Terms of Use</a> and
							confirm you have read our
							<a href="#" class="underline dark:text-gray-300">Privacy and Cookie Statement</a>.
						</p>
						<p class="text-xs dark:text-gray-300">
							This site is protected by reCAPTCHA and the <a href="#" class="underline"
								>Google Privacy Policy</a
							>
							and <a href="#" class="underline dark:text-gray-300">Terms of Service</a> apply.
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
<!-- <div class="icons8-microsoft"></div>
		<div class="icons8-google"></div> -->
