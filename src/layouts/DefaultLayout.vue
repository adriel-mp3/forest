<script setup lang="ts">
import MainHeader from "@/components/ui/MainHeader.vue";
import WeatherWidget from "@/components/ui/WeatherWidget.vue";
</script>

<template>
	<div class="h-screen">
		<div class="flex flex-col">
			<WeatherWidget />
			<MainHeader />
			<slot />
		</div>
	</div>
</template>
