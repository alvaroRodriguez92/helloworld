<template>
<ul>
    <li v-for="(country,index) in countries" v-bind:key="index">{{ country.name }}</li>
</ul>
</template>

<script lang="ts" setup>
import {Ref, ref} from 'vue'

interface Country{
code:string,
name:string
}

let countries :Ref<Array<Country>>= ref([
    {
        code:"es",
        name:"Spain"
    },{
        code:"en",
        name:"UK"
    },{
        code:"fr",
        name:"France"
    },{
        code:"it",
        name:"Italy"
    },{
        code:"pt",
        name:"Portugal"
    },
])
</script>