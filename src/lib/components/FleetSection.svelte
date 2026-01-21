<script lang="ts">
	import atvRed from '$lib/assets/atvs/atv-red.png';
	import atvBlue from '$lib/assets/atvs/atv-blue.png';
	import atvSmall from '$lib/assets/atvs/atv-small.png';
</script>

<section class="py-20 bg-white">
	<div class="container mx-auto px-6">
		<h2 class="text-3xl md:text-3xl text-center text-blue-600 mb-12 uppercase tracking-wide">Rides Start From Rs 500/- to 1200/- Based on ATV Size, Solo/Double Rides For Duration of 15 minutes or 5 Laps Around The Farm</h2>

		<div class="grid grid-cols-1 md:grid-cols-3 gap-10">
			<!-- 300cc ATV (Red) -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col">
				<div class="aspect-square overflow-hidden rounded-t-2xl">
					<img
						src={atvRed}
						alt="300cc Red ATV"
						class="size-full object-cover object-center"
					/>
				</div>
				<div class="p-6">
					<h3 class="text-3xl mb-4">300cc ATV</h3>
					<p class="text-lg">
						High-performance ATV suitable for single or double riders.
						<strong class="block mt-4">Rates:</strong>
						₹800 — Single rider<br />
						₹1200 — Double riders
					</p>
				</div>
			</div>

			<!-- 135cc ATV (Blue) -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col">
				<div class="aspect-square overflow-hidden rounded-t-2xl">
					<img
						src={atvBlue}
						alt="135cc  Blue ATV"
						class="size-full object-cover object-center"
					/>
				</div>
				<div class="p-6">
					<h3 class="text-3xl mb-4">135cc ATV</h3>
					<p class="text-lg">
						Suitable for teenagers seeking a thrilling ride.
						<strong class="block mt-4">Rates:</strong>
						₹600 — Single rider<br />
					</p>
				</div>
			</div>

			<!-- Beginner ATV -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col">
				<div class="aspect-square overflow-hidden rounded-t-2xl">
					<img
						src={atvSmall}
						alt="Beginner ATV"
						class="size-full object-cover object-center"
					/>
				</div>
				<div class="p-6">
					<h3 class="text-3xl mb-4">Beginner ATV</h3>
					<p class="text-lg">
						Perfect for first-timers, younger riders or those wanting a gentler experience.
						<strong class="block mt-4">Rates:</strong>
						₹500 — Single rider
					</p>
				</div>
			</div>
		</div>
	</div>
</section>