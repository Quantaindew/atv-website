<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import logo from '$lib/assets/atv-logo.jpg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} type="image/svg+xml" />
</svelte:head>

<header class="bg-blue-800 text-white shadow-md sticky top-0 z-50">
	<div class="max-w-7xl mx-auto px-6 py-4 text-center relative">
		<img
			src={logo}
			alt="The ATV Club Logo"
			class="absolute left-4 top-1/2 -translate-y-1/2 h-10 w-10 md:left-6 md:h-12 md:w-12 rounded-full object-cover shadow-lg"
		/>
		<h1 class="text-3xl font-bold uppercase tracking-wider">The ATV Club</h1>
	</div>
</header>

<div class="min-h-screen">
	{@render children()}
</div>

<footer class="bg-gray-900 text-white py-10 mt-20 relative">
	<div class="max-w-7xl mx-auto px-6 text-center space-y-4 relative">
		<img
			src={logo}
			alt="The ATV Club Logo"
			class="absolute left-4 top-10 h-16 w-16 md:left-6 md:h-20 md:w-20 rounded-full object-cover shadow-2xl"
		/>
		<h3 class="text-2xl font-bold uppercase">The ATV Club</h3>
		<p>
			<a
				href="https://maps.app.goo.gl/xnFUpxmpuPMzmeDv6"
				target="_blank"
				rel="noopener"
				class="hover:underline">@ Q C Farm (Taájem),<br />Near Bogmalo Church,<br />Bogmalo - Goa</a
			>
		</p>
		<p class="text-lg">
			WhatsApp / Call: <a href="tel:+919423322588" class="hover:underline">+91 94233 22588</a>
		</p>
		<p>
			Instagram: <a
				href="https://www.instagram.com/the_atv_club"
				target="_blank"
				rel="noopener"
				class="hover:underline">the_atv_club</a
			>
		</p>
		<p class="text-sm mt-6">&copy; {new Date().getFullYear()} theatvclubgoa.in. All rights reserved.</p>
	</div>
</footer>