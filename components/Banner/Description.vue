<template>
        <p class="text-white text-center font-medium mb-8">{{text}}</p>
</template>

<script setup lang="ts">
interface props {
    text: string 
}
const props = defineProps<props>()
</script>
