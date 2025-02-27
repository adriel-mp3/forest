<script setup lang="ts">
import WeatherWidget from "@/components/WeatherWidget.vue";
</script>

<template>
	<div class="h-screen">
		<WeatherWidget />
		<slot />
	</div>
</template>
