<script setup lang="ts">
defineProps<{
	text: string;
	buttonText: string;
	buttonLink?: string;
}>();
</script>

<template>
	<div
		class="sm:bg-neutral-green-900 bg-neutral-green-900/60 mb-8 flex flex-col items-start gap-2 rounded-xl p-4 sm:inline-flex sm:flex-row sm:items-center sm:gap-8 sm:rounded-full sm:py-1 sm:pr-1 sm:pl-4"
	>
		<span>{{ text }}</span>
		<a
			:href="buttonLink || '#'"
			class="bg-forest-green-900 text-moss-green-900 inline-block cursor-pointer rounded-full px-4 py-2"
		>
			{{ buttonText }}
		</a>
	</div>
</template>
