<script setup lang="ts">
import type { IMainMenuNavItem } from "@/types";
import MainMenuNavItem from "./MainMenuNavItem.vue";

defineProps<{
	items: IMainMenuNavItem[];
}>();
</script>

<template>
	<ul class="flex gap-8">
		<li v-for="item in items" :key="item.to">
			<MainMenuNavItem :item="item" />
		</li>
	</ul>
</template>
