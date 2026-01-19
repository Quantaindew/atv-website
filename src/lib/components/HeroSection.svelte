<script lang="ts">
	import { onMount } from 'svelte';

	import carousel0 from '$lib/assets/carousel-0.jpg';
	import carousel1 from '$lib/assets/carousel-1.jpg';
	import carousel2 from '$lib/assets/carousel-2.jpg';
	import carousel3 from '$lib/assets/carousel-3.jpg';

	const images = [carousel0, carousel1, carousel2, carousel3] as const;

	let currentIndex = 0;

	onMount(() => {
		const interval = setInterval(() => {
			currentIndex = (currentIndex + 1) % images.length;
		}, 6000);

		return () => clearInterval(interval);
	});
</script>

<section class="relative h-[80vh] md:h-screen flex items-center justify-center text-white overflow-hidden">
	<!-- Carousel images -->
	{#each images as src, index}
		<img
			src={src}
			alt="Thrilling ATV ride in Goa"
			class="absolute inset-0 w-full h-full object-cover object-center transition-opacity duration-2000 ease-in-out {currentIndex ===
			index
				? 'opacity-100'
				: 'opacity-0'}"
		/>
	{/each}

	<!-- Dark overlay -->
	<div class="absolute inset-0 bg-black/60"></div>

	<!-- Hero content -->
	<div class="relative z-10 container mx-auto px-6 text-center">
		<h1 class="text-5xl md:text-7xl mb-6 drop-shadow-2xl uppercase tracking-wider">
			The ATV Club
		</h1>
		<p class="text-2xl md:text-3xl mb-4 drop-shadow-lg">Thrilling Off-Road Adventures</p>
		<p class="text-xl md:text-2xl mb-10 drop-shadow-lg">Bogmalo, Goa</p>
		<div class="flex flex-col md:flex-row gap-6 justify-center">
			<a
				href="https://wa.me/919423322588?text=Hello!%20I'm%20interested%20in%20ATV%20rides%20at%20The%20ATV%20Club."
				class="btn-whatsapp text-xl"
			>
				Chat on WhatsApp
			</a>
			<a href="tel:+919423322588" class="btn-primary text-xl">Call Us Now</a>
		</div>
	</div>

	<!-- Carousel indicators -->
	<div class="absolute bottom-8 left-1/2 -translate-x-1/2 flex space-x-3 z-20">
		{#each images as _, i}
			<button
				type="button"
				on:click={() => (currentIndex = i)}
				class="w-3 h-3 rounded-full transition-all {currentIndex === i
					? 'bg-white scale-125'
					: 'bg-white/50 hover:bg-white'}"
				aria-label="Go to slide {i + 1}"
			></button>
		{/each}
	</div>
</section>