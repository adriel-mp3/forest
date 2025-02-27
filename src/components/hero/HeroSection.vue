<script setup lang="ts">
import BestPlaces from "./BestPlaces.vue";
import HeroActionBanner from "./HeroActionBanner.vue";
import RecommendedBy from "./RecommendedBy.vue";
</script>

<template>
	<main class="z-0 container">
		<div
			class="from-neutral-green-900/80 relative overflow-hidden rounded-2xl bg-gradient-to-t px-4 pt-12 pb-8 text-white sm:px-8 sm:pt-64"
		>
			<img
				class="absolute inset-0 -z-10 size-full object-cover"
				src="/img/wild-forest.jpg"
			/>
			<HeroActionBanner
				text="vagas para dezembro abertas"
				button-text="Reserve Hoje"
			/>
			<h1 class="mb-8 sm:mb-20 max-w-screen-sm font-serif text-4xl sm:text-5xl text-balance">
				Venha Experimentar a Vida na floresta
			</h1>
			<div class="sm:flex items-end justify-between">
				<BestPlaces year="2048" />
				<RecommendedBy
					logo-src="/img/partners/wildbeast.svg"
					logo-alt="Logo Wildbeast"
					publication="Revista nacional"
				/>
			</div>
		</div>
	</main>
</template>
