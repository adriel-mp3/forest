<script setup lang="ts">
import type { IMainMenuNavItem } from "@/types";
import MainMenuNav from "./MainMenuNav.vue";
import ForestLogo from "@/components/icons/ForestLogo.vue";

const menuItems = [
	{
		to: "#",
		label: "Acomodações",
	},
	{
		to: "#",
		label: "Eventos",
	},
	{
		to: "#",
		label: "Experiências",
	},
	{
		to: "#",
		label: "Contato",
	},
] satisfies IMainMenuNavItem[];
</script>

<template>
	<header class="container flex items-center justify-between">
		<ForestLogo />
		<MainMenuNav :items="menuItems" />
	</header>
</template>
