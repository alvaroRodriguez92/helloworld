<template>
<h1 v-if="age < 18">Eres menor de edad</h1>
<h1 v-else-if="age>=18">Eres mayor de edad</h1>
<h3>{{ age }}</h3>
<button @click="changeAge">Cambiar edad</button>
</template>

<script lang="ts" setup>
import {ref} from "vue"
        let age= ref(10);
        const changeAge = ()=>{
            console.log(age)

            if(age.value<18){
                age.value = 20
            } else if(age.value>17){
                age.value=10
            }
        }
</script>

<style scoped>
</style>