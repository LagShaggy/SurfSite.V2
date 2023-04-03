<script>
	import '../app.postcss';
	export const ssr = false;
	export let img = '/oe26_logo.svg';

	import Navbar from '$lib/components/UI/Navbar.svelte';
	import Footer from '$lib/components/UI/Footer.svelte';

	let nr = 3;
</script>

<Navbar />

<div class="h-full flex justify-center mt-5 mb-2 shadow-lg">
	<slot />
</div>

<a href="/home" class="mt-1 h-screen flex items-center justify-center">
	<div class="absolute">
		<img src={img} alt="OE26" class="opacity-20 object-cover h-full" />
	</div>
</a>

<Footer />
