<script lang="ts">
	import atvRed from '$lib/assets/atvs/atv-red.png';
	import atvBlue from '$lib/assets/atvs/atv-blue.png';
	import atvSmall from '$lib/assets/atvs/atv-small.png';
</script>

<section class="py-20 bg-gray-100">
	<div class="container mx-auto px-6">
		<h2 class="text-4xl md:text-5xl text-center text-blue-600 mb-12 uppercase tracking-wide">Rides Start From Rs 500/- to 1200/- Based on ATV Size, Solo/Double Rides For Duration of 15 minutes (5 Laps Around The Farm)</h2>
		<div class="grid grid-cols-1 md:grid-cols-3 gap-10">
			<!-- 300cc Red ATV -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col aspect-[610/987]">
				<div class="aspect-square">
					<img
						src={atvRed}
						alt="300cc Red ATV"
						class="size-full object-cover"
					/>
				</div>
				<div class="p-6 flex-1">
					<h3 class="text-3xl mb-4">300cc ATV</h3>
					<p class="text-lg">
						High-performance ATV suitable for single or double riders.
						<strong class="block mt-4">Rates (5 laps):</strong>
						₹800 — Single rider<br />
						₹1200 — Double riders
					</p>
				</div>
			</div>

			<!-- High-Performance Blue ATV -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col aspect-[610/987]">
				<div class="aspect-square">
					<img
						src={atvBlue}
						alt="135cc  Blue ATV"
						class="size-full object-cover"
					/>
				</div>
				<div class="p-6 flex-1">
					<h3 class="text-3xl mb-4">135cc ATVs</h3>
					<p class="text-lg">
						Suitable for teenagers seeking a thrilling ride.
						<strong class="block mt-4">Rates (5 laps):</strong>
						₹600 — Single rider
					</p>
				</div>
			</div>

			<!-- 125cc Small ATV -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col aspect-[610/987]">
				<div class="aspect-square">
					<img
						src={atvSmall}
						alt="125cc Small ATV"
						class="size-full object-cover"
					/>
				</div>
				<div class="p-6 flex-1">
					<h3 class="text-3xl mb-4">110cc ATV</h3>
					<p class="text-lg">
						Beginner-friendly ATV, perfect for first-timers and families.
						<strong class="block mt-4">Rates (5 laps):</strong>
						₹600 — Single rider
					</p>
				</div>
			</div>
		</div>
	</div>
</section>