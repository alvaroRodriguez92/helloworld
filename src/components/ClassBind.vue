<template>
    <p v-bind:style="{
        'backgroundColor':'green', color:color, border:'1px solid red', padding:'24px'
    }">El mensaje se ha enviado correctamente.</p>
    <button v-on:click="handleClick">Cambiar color</button>
</template>

<script lang="ts" setup>
import {ref} from "vue"
let color=ref('blue')

const handleClick = ()=>{
    color.value=='blue'? color.value='white' : color.value='blue'
}
</script>

<style scoped>

</style>