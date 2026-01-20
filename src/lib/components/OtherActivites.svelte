<script lang="ts">
	import beach from '$lib/assets/otheractivities/beach.png';
	import atvBlue from '$lib/assets/atvs/atv-blue.png';
	import atvSmall from '$lib/assets/atvs/atv-small.png';
</script>

<section class="py-20 bg-white">
	<div class="container mx-auto px-6">
		<h2 class="text-5xl md:text-5xl text-center text-blue-600 mb-12 uppercase tracking-wide">Other Activities</h2>
		<h2 class="text-3xl md:text-3xl text-center text-blue-600 mb-12 uppercase tracking-wide">We also cater to special requests like beach rides, couple entry for Weddings/Haldi/Anniversaries/Birthdays and other functions.</h2>
		<div class="grid grid-cols-1 md:grid-cols-3 gap-10">
			<!-- 300cc Beach ATV -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col aspect-[610/987]">
				<div class="aspect-square">
					<img
						src={beach}
						alt="300cc Beach ATV"
						class="size-full object-cover"
					/>
				</div>
				<div class="p-6 flex-1">
					<h3 class="text-3xl mb-4">Beach Rides with 500cc 4 Wheel Drive ATVs</h3>
					<p class="text-lg">
						<strong class="block mt-4">Rates (15 Mins):</strong>
							₹2000 — Single <br />
							₹3000 — Double
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
						<strong class="block mt-4">Rates:</strong>
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
						<strong class="block mt-4">Rates:</strong>
						₹600 — Single rider
					</p>
				</div>
			</div>
		</div>
	</div>
</section>