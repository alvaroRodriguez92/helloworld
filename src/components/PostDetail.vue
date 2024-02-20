<template>
<div class="post">
    <h3>{{title}}</h3>
    <p>{{content}}</p>
    <input placeholder="Escribe tu saludo" v-model="message"/><button @click="sayHiFromChild">Di hola</button>
</div>
</template>

<script lang="ts">
import {defineComponent, ref, Ref} from 'vue'
export default defineComponent({
    name:"PostDetail",
    props:{
        title:{
            type:String,
            required:true
        },
        content:{
            type:String,
            required:true
        }
    },
    emits:["sayHi"],
    setup(props, {emit}){
        const message: Ref<string> = ref("")

        const sayHiFromChild = ()=>{
            emit("sayHi", message.value)
        }
        return {props, sayHiFromChild, message}
    }
})

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

