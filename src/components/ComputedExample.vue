<template>
<div><input type="text" v-model="message"/>
<h3>{{ message }}</h3></div>
</template>

<script lang="ts" setup>
import{Ref, ref} from 'vue'

const message:Ref<string> =ref("")

</script>

<style scoped>
</style>

