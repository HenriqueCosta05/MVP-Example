<template>
        <h1 class="text-white text-center font-bold text-7xl my-4">{{text}}<span class="text-[#FBA45A] block">{{highlightedText}}</span></h1>
</template>

<script setup lang="ts">
interface props {
    text: string;
    highlightedText: string;
}
const props = defineProps<props>()
</script>
