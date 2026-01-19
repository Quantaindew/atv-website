<script lang="ts">
	import atvRed from '$lib/assets/atvs/atv-red.jpg';
	import atvBlue from '$lib/assets/atvs/atv-blue.jpg';
	import atvYellow from '$lib/assets/atvs/atv-yellow.jpg';
</script>

<section class="py-20 bg-gray-100">
	<div class="container mx-auto px-6">
		<h2 class="text-4xl md:text-5xl text-center text-blue-600 mb-12 uppercase tracking-wide">Our Fleet</h2>
		<div class="grid grid-cols-1 md:grid-cols-3 gap-10">
			<!-- 300cc Red ATV -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col">
				<img
					src={atvRed}
					alt="300cc Red ATV"
					class="w-full h-64 object-cover"
				/>
				<div class="p-8 flex-1">
					<h3 class="text-3xl mb-4">300cc ATV (Red)</h3>
					<p class="text-lg">
						High-performance ATV suitable for single or double riders.<br /><br />
						<strong>Rates (5 laps):</strong><br />
						₹800 — Single rider<br />
						₹1000 — Double riders
					</p>
				</div>
			</div>

			<!-- 125cc Blue ATV -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col">
				<img
					src={atvBlue}
					alt="125cc Blue ATV"
					class="w-full h-64 object-cover"
				/>
				<div class="p-8 flex-1">
					<h3 class="text-3xl mb-4">125cc ATV (Blue)</h3>
					<p class="text-lg">
						Beginner-friendly ATV, perfect for first-timers and families.<br /><br />
						<strong>Rates (5 laps):</strong><br />
						₹600 — Single rider<br />
						₹800 — Double riders
					</p>
				</div>
			</div>

			<!-- Yellow ATV (assumed high-performance, same pricing as red since no separate notes) -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col">
				<img
					src={atvYellow}
					alt="High-performance Yellow ATV"
					class="w-full h-64 object-cover"
				/>
				<div class="p-8 flex-1">
					<h3 class="text-3xl mb-4">High-Performance ATV (Yellow)</h3>
					<p class="text-lg">
						Powerful ATV for thrilling single or double rider adventures.<br /><br />
						<strong>Rates (5 laps):</strong><br />
						₹800 — Single rider<br />
						₹1000 — Double riders
					</p>
				</div>
			</div>
		</div>
	</div>
</section>