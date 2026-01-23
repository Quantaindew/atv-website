<script lang="ts">
	import beach from '$lib/assets/otheractivities/beach.png';
	import atvFilm from '$lib/assets/otheractivities/film.png';
	import atvWeddings from '$lib/assets/otheractivities/weddings.jpg';
</script>

<section class="py-20 bg-white">
	<div class="container mx-auto px-6">
		<h2 class="text-5xl md:text-5xl text-center text-blue-600 mb-12 uppercase tracking-wide">Other Activities</h2>
		<h2 class="text-3xl md:text-3xl text-center text-blue-600 mb-12 uppercase tracking-wide">
			We also cater to special requests like beach rides, couple entry for Weddings/Haldi, Anniversaries, Birthdays and other functions.
		</h2>
		<div class="grid grid-cols-1 md:grid-cols-3 gap-10">
			<!-- Beach Rides -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col">
				<div class="aspect-square overflow-hidden rounded-t-2xl">
					<img
						src={beach}
						alt="500cc 4WD Beach ATV"
						class="size-full object-cover object-center"
					/>
				</div>
				<div class="p-6">
					<h3 class="text-3xl mb-4">Beach Rides with 500cc 4 Wheel Drive ATVs</h3>
					<p class="text-lg">
						<strong class="block mt-4">Rates (20 Mins):</strong>
						₹2000 — Single <br />
						₹3000 — Double <br />
						<br />
						Location: Baina Beach, Vasco Da Gama, Goa.
					</p>
				</div>
			</div>

			<!-- Film Shoots -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col">
				<div class="aspect-square overflow-hidden rounded-t-2xl">
					<img
						src={atvFilm}
						alt="ATV for Film Shoots"
						class="size-full object-cover object-center"
					/>
				</div>
				<div class="p-6">
					<h3 class="text-3xl mb-4">Films Shoots</h3>
					<p class="text-lg">
						<strong class="block mt-4">Rates:</strong>
						₹20,000 For First 2 hours <br />
						Inclusive of operator, fuel and transportation to any location in Goa. <br /> 
						Thereafter ₹5,000 for every additional hour.
					</p>
				</div>
			</div>

			<!-- Weddings/Haldi/Anniversary -->
			<div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col">
				<div class="aspect-square overflow-hidden rounded-t-2xl">
					<img
						src={atvWeddings}
						alt="ATV for Wedding Entry"
						class="size-full object-cover object-center"
					/>
				</div>
				<div class="p-6">
					<h3 class="text-3xl mb-4">Weddings/Haldi Anniversaries Birthdays</h3>
					<p class="text-lg">
						<strong class="block mt-4">Rates:</strong>
						₹15,000 For First 2 hours <br />
						Inclusive of operator, fuel and transportation to any location in Goa. <br /> 
						Thereafter ₹5,000 for every additional 2 hours.
					</p>
				</div>
			</div>
		</div>
	</div>
</section>