<script lang="ts">
	import { page } from "$app/state";
</script>

<main class="min-h-screen flex items-center justify-center bg-gray-50 px-6">
	<div class="text-center max-w-md">
		<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-16 h-16 text-primary-600 mx-auto mb-6">
			<path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z" fill="currentColor" />
		</svg>
		<h1 class="text-6xl font-serif text-gray-900 mb-4">{page.status}</h1>
		<p class="text-lg text-gray-600 mb-8">{page.error?.message ?? "Something went wrong."}</p>
		<a href="/" class="inline-block bg-primary-950 text-white px-8 py-3.5 rounded-full font-medium text-sm hover:bg-primary-900 transition-colors">
			Return Home
		</a>
	</div>
</main>
