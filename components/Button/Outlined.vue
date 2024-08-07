<template>
      <button
    class="align-middle select-none font-sans font-bold text-center uppercase transition-all disabled:opacity-50 disabled:shadow-none disabled:pointer-events-none text-xs py-3 px-6 rounded-lg border border-[#FBA45A] text-white hover:opacity-75 focus:ring focus:ring-gray-300 active:opacity-[0.85] flex items-center gap-3"
    type="button">
    <img :src="props.icon" alt="icon" class="w-4 h-4" />
    {{text}}
  </button>
</template>

<script setup lang="ts">
import type { ButtonProps } from '~/types/props/button';


const props = defineProps<ButtonProps>()
</script>
