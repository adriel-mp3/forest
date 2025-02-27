<script setup lang="ts">
defineProps<{
	year: string;
	link?: string;
}>();
</script>

<template>
	<p class="max-sm:mb-4">
		Melhores locais para visitar
		<a
			class="underline decoration-2 underline-offset-4 hover:no-underline"
			:href="link || '#'"
		>
			{{ year }}
		</a>
	</p>
</template>
