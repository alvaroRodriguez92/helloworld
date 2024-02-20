<template>
<div class="post">
    <h3>{{props.title}}</h3>
    <p>{{props.content}}</p>
    <input placeholder="Escribe tu saludo" v-model="message"/><button @click="sayHiFromChild">Di hola</button>
</div>
</template>

<script lang="ts" setup>
import {defineProps,defineEmits, ref, Ref} from 'vue'
    const props = defineProps({
        title:String,
        content:String
    })
    const emit = defineEmits(["sayHi"])
        const message: Ref<string> = ref("")

        const sayHiFromChild = ()=>{
            emit("sayHi", message.value)
           }

</script>

<style scoped>
.post{
    width: 304px;
    height:160px;
    background-color: antiquewhite;
    border-radius: 16px;
    border: 1px solid salmon;
    margin: 8px;
    padding: 8px;
}
</style>

