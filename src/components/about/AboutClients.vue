<script>
import AboutClientSingle from './AboutClientSingle.vue';

export default {
	components: {
		AboutClientSingle,
	},
	data: () => {
		return {
			clientsHeading: 'Some of the brands I have worked with',
			clients: [
				{
					id: 1,
					title: 'BenQ',
					img: require('@/assets/images/brands/Benq.png'),
				},
				{
					id: 2,
					title: 'KotakGame',
					img: require('@/assets/images/brands/kotakgame.png'),
				},
				{
					id: 3,
					title: 'NJT',
					img: require('@/assets/images/brands/LogoNJT.png'),
				},
				{
					id: 4,
					title: 'Cooler Master',
					img: require('@/assets/images/brands/CM Logo Tagline Right Black RGB.png'),
				},
				{
					id: 5,
					title: '"Klevv"',
					img: require('@/assets/images/brands/klevv.png'),
				},
				{
					id: 6,
					title: 'MyClubGaming',
					img: require('@/assets/images/brands/MyClubGaming.png'),
				},
				{
					id: 7,
					title: 'Palit',
					img: require('@/assets/images/brands/logo_palit.png'),
				},
				{
					id: 7,
					title: 'Asus',
					img: require('@/assets/images/brands/asus.png'),
				},
			],
		};
	},
};
</script>

<template>
	<div class="mt-10 sm:mt-20">
		<p
			class="font-general-medium text-2xl sm:text-3xl text-primary-dark dark:text-primary-light"
		>
			{{ clientsHeading }}
		</p>
		<div class="grid grid-cols-2 sm:grid-cols-4 mt-10 sm:mt-14 gap-2">
			<AboutClientSingle
				v-for="client in clients"
				:key="client.id"
				:client="client"
			/>
		</div>
	</div>
</template>
