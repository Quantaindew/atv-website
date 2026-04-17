<script lang="ts">
	import { onMount } from 'svelte';

	import carousel0 from '$lib/assets/carousel/carousel-0.jpg';
	import carousel1 from '$lib/assets/carousel/carousel-1.jpg';
	import carousel2 from '$lib/assets/carousel/carousel-2.jpg';
	import carousel3 from '$lib/assets/carousel/carousel-3.jpg';

	const images = [carousel0, carousel1, carousel2, carousel3] as const;

	let currentIndex = 0;

	let startX: number | null = null;
	let startY: number | null = null;

	const handleTouchStart = (e: TouchEvent) => {
		startX = e.touches[0].clientX;
		startY = e.touches[0].clientY;
	};

	const handleTouchMove = (e: TouchEvent) => {
		if (startX === null || startY === null) return;

		const currentX = e.touches[0].clientX;
		const currentY = e.touches[0].clientY;

		const deltaX = Math.abs(currentX - startX);
		const deltaY = Math.abs(currentY - startY);

		// Prevent vertical page scroll only if horizontal swipe is clearly intended
		if (deltaX > deltaY && deltaX > 20) {
			e.preventDefault();
		}
	};

	const handleTouchEnd = (e: TouchEvent) => {
		if (startX === null) return;

		const endX = e.changedTouches[0].clientX;
		const distance = startX - endX;
		const threshold = 50;

		if (Math.abs(distance) >= threshold) {
			if (distance > 0) {
				// Swipe left → next
				currentIndex = (currentIndex + 1) % images.length;
			} else {
				// Swipe right → previous
				currentIndex = (currentIndex + images.length - 1) % images.length;
			}
		}

		startX = null;
		startY = null;
	};

	onMount(() => {
		const interval = setInterval(() => {
			currentIndex = (currentIndex + 1) % images.length;
		}, 6000);

		return () => clearInterval(interval);
	});
</script>

<section
	class="relative h-[80vh] md:h-screen text-white overflow-hidden touch-pan-y"
	ontouchstart={handleTouchStart}
	ontouchmove={handleTouchMove}
	ontouchend={handleTouchEnd}
>
	<!-- Carousel images (fade transition) -->
	{#each images as src, index}
		<img
			src={src}
			alt="Thrilling ATV ride in Goa"
			class="absolute inset-0 w-full h-full object-cover object-center transition-opacity duration-1000 ease-in-out {currentIndex ===
			index
				? 'opacity-100'
				: 'opacity-0'}"
		/>
	{/each}

	<!-- Bottom gradient for text legibility only -->
	<div class="absolute inset-x-0 bottom-0 h-56 md:h-72 bg-linear-to-t from-black/80 via-black/40 to-transparent pointer-events-none"></div>

	<!-- Hero content – compact and at the bottom -->
	<div class="absolute inset-x-0 bottom-0 z-10 container mx-auto px-6 pb-6 md:pb-10 text-center">
		<h1 class="text-3xl md:text-5xl mb-2 drop-shadow-2xl uppercase tracking-wider">
			Thrilling Off-Road Adventures
		</h1>
		<p class="text-lg md:text-2xl mb-4 drop-shadow-lg">Bogmalo, Goa</p>

		<div class="flex flex-col md:flex-row gap-4 justify-center mb-5">
			<a
				href="https://wa.me/919423322588?text=Hi!%20I%27d%20like%20to%20book%20an%20ATV%20adventure%20at%20The%20ATV%20Club."
				class="btn-whatsapp py-2.5 px-6 text-base md:text-lg"
			>
				Click to Book via WhatsApp
			</a>
			<a href="tel:+919423322588" class="btn-primary py-2.5 px-6 text-base md:text-lg">
				Click to Book via Call
			</a>
		</div>

		<!-- Indicators -->
		<div class="flex space-x-3 justify-center">
			{#each images as _, i}
				<button
					type="button"
					onclick={() => (currentIndex = i)}
					class="w-2.5 h-2.5 rounded-full transition-all {currentIndex === i
						? 'bg-white scale-125'
						: 'bg-white/50 hover:bg-white'}"
					aria-label="Go to slide {i + 1}"
				></button>
			{/each}
		</div>
	</div>
</section>