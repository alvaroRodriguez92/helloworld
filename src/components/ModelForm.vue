<template>
    <h1>Formulario muy guapo</h1>
    <form>
        <input type="text" v-model="inputText"/><br><br>
        <input type="checkbox" v-model="agree">Acepto condiciones y términos.<br>
        <select v-model="country">
            <option value="Spain">Spain</option>
            <option value="UK">UK</option>
            <option value="France">France</option>
        </select>
</form>

    <h3>{{ inputText }}</h3>
    <h3>Valor de variable agree: {{ agree }}</h3>
    <h3>Valor de variable country: {{ country }}</h3>
</template>

<script lang="ts" setup>
import {ref} from 'vue'

let inputText= ref('')
let agree= ref(false)
let country = ref('Spain')
</script>

<style scoped>
h1{
    color:brown
}
</style>