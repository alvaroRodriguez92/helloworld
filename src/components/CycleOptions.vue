<template>
<h1>Hola k ase</h1>
</template>

<script lang="ts" setup>
import { onMounted, onUpdated } from 'vue';
onMounted(() => {
    console.log("Montadoo")
})

onUpdated(() => {
    console.log("Updateando")
})

</script>

<style scoped>
</style>

