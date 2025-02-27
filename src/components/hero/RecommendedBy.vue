<script setup lang="ts">
defineProps<{
  logoSrc: string;
  logoAlt?: string;
  publication: string;
}>();
</script>

<template>
  <div>
    <p class="mb-2 uppercase">Recomendado por</p>
    <div class="flex items-center gap-4">
      <img class="w-28" :src="logoSrc" :alt="logoAlt || 'Logo recomendação'" />
      <span>|</span>
      <span class="text-sm capitalize">{{ publication }}</span>
    </div>
  </div>
</template>
