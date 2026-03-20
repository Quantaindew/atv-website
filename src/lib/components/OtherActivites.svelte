<script lang="ts">
	import atvFilm from '$lib/assets/otheractivities/film.png';
	import atvWeddings from '$lib/assets/otheractivities/weddings.jpg';
</script>

<section class="py-20 bg-white">
	<div class="container mx-auto px-6">
		<h2 class="text-5xl md:text-5xl text-center text-blue-600 mb-12 uppercase tracking-wide">Other Activities</h2>
		<h2 class="text-3xl md:text-3xl text-center text-blue-600 mb-12 uppercase tracking-wide">
			We also cater to special requests like film shoots, couple entry for Weddings/Haldi, Anniversaries, Birthdays and other functions.
		</h2>
		<div class="grid grid-cols-1 md:grid-cols-2 gap-10">
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