<script lang="ts">
	import atvRed from '$lib/assets/atvs/atv-red.png';
	import atvBlue from '$lib/assets/atvs/atv-blue.png';
	import atvSmall from '$lib/assets/atvs/atv-small.png';
</script>

<section class="py-20 bg-white">
	<div class="container mx-auto px-6">
		<h2 class="text-5xl md:text-5xl text-center text-blue-600 mb-12 uppercase tracking-wide">Around the Farm</h2>

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

			<!-- 300cc ATV (Blue) -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col">
				<div class="aspect-square overflow-hidden rounded-t-2xl">
					<img
						src={atvBlue}
						alt="300cc Blue ATV"
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
						₹600 — Single rider
					</p>
				</div>
			</div>
		</div>
	</div>
</section>