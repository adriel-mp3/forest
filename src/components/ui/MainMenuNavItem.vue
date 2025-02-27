<script setup lang="ts">
import type { IMainMenuNavItem } from "@/types";

defineProps<{
	item: IMainMenuNavItem;
}>();
</script>

<template>
	<a
		class="text-xl text-white underline-offset-6 hover:underline"
		:href="item.to"
	>
		{{ item.label }}
	</a>
</template>
