<script setup lang="ts">
const widgetItems = {
	dayOfWeek: "Quarta",
	day: 24,
	umidity: 29,
};
</script>

<template>
	<div class="container flex items-center justify-center md:justify-start">
		<span class="bg-forest-green-900 relative -right-1 size-2 rounded-full">
		</span>
		<ul
			class="bg-moss-green-900 text-forest-green-900 divide-moss-green-800 inline-flex items-center justify-center divide-x-2 rounded"
		>
			<li class="px-4 py-2 pl-6 capitalize">{{ widgetItems.dayOfWeek }}</li>
			<li class="px-4 py-2 capitalize">{{ widgetItems.day }}º</li>
			<li class="px-4 py-2 capitalize">🌧️ {{ widgetItems.umidity }}%</li>
		</ul>
	</div>
</template>
