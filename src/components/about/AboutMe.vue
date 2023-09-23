<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						'Lulusan Rekayasa Perangkat Lunak (RPL) SMKS Babunnajah. Saya tertarik untuk melamar dibidang IT, Web Developer, dan Graphic Designer. Sangat termotivasi dalam belajar hal baru, membangun inovasi, berkarya dalam industri Graphic Designer dan Web Developer, serta bekerjasama dengan Partner. Dilengkapi dengan pengalaman dan sertifikat yang relevan.',
				},

			],
		};
	},
};
</script>

<template>

	
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/profile1.png"
				class="rounded-xl"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<h1 class="font-general-semibold text-3xl md:text-3xl xl:text-4xl text-center sm:text-left text-ternary-dark dark:text-primary-light uppercase">Shevcenko Radjartha</h1>
			<p
				class="font-general-medium mt-2 text-lg sm:text-xl  xl:text-2xl text-center sm:text-left leading-none text-gray-400"
			>
			IT, Web Developer, Graphic Designer.
			</p>
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="text-center sm:text-left font-general-regular pt-2 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
