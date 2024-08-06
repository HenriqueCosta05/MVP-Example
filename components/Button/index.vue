<template>
     <button
    class="align-middle select-none font-sans font-bold text-center uppercase transition-all disabled:opacity-50 disabled:shadow-none disabled:pointer-events-none text-xs py-3 px-6 rounded-lg bg-[#FBA45A] text-white shadow-md shadow-gray-300/10 hover:shadow-lg hover:shadow-gray-900/20 focus:opacity-[0.85] focus:shadow-none active:opacity-[0.85] active:shadow-none flex items-center gap-3"
    type="button">
    <img :src="icon" alt="rocket" class="w-4 h-4" />
    {{ text }}
  </button>
</template>

<script setup lang="ts">
import type { ButtonProps } from '~/types/props/button';

const props = defineProps<ButtonProps>()

</script>
