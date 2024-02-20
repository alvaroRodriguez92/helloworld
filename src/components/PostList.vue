<template>
<div class="postlist-container">
<PostDetail v-for="(item, index) in info" v-bind:key="index" :title ="item.title" :content="item.content" @sayHi="showAlert"/>
</div>
</template>

<script lang="ts" setup>
import PostDetail from './PostDetail.vue'

interface Info{
title:string,
content:string
}

const info :Info[] = [{
    title:"Este es el post 1",
    content:"Texto de ejemplo 1"
},{
    title:"Este es el post 2",
    content:"Texto de ejemplo 2"
},{
    title:"Este es el post 3",
    content:"Texto de ejemplo 3"
},{
    title:"Este es el post 4",
    content:"Texto de ejemplo 4"
},{
    title:"Este es el post 5",
    content:"Texto de ejemplo 5"
}]

function showAlert(msg:string){
    alert(msg)
}

</script>

<style scoped>
.postlist-container{
    display:flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-around;
}
</style>

