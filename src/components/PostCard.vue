<template>
<div class="post-card">
    <h3>Título</h3>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi expedita ratione eligendi vitae, obcaecati sed doloremque accusantium, sit aperiam quibusdam delectus mollitia eius facere sint reiciendis quis blanditiis quod unde recusandae esse voluptatum? Nam id iste quis adipisci dolorem vero, quam rem eveniet repellendus veritatis quae dolores fugiat tempore, ipsum voluptas ex, ipsam illum voluptatibus sed minima aliquid! Quasi distinctio ipsum fugiat repellendus aut possimus assumenda fugit consectetur, iure sit nulla exercitationem, itaque repudiandae magni aliquid dicta? Dignissimos, debitis? Magni quidem accusantium laboriosam pariatur sunt? Porro placeat et quia sint expedita velit tenetur, voluptates accusantium fuga laborum fugiat, libero dolorum!</p>
    <PostButton/>
</div>
</template>

<script lang="ts" setup>
import PostButton from './PostButton.vue';
</script>

<style scoped>
.post-card{
    border-radius: 16px;
    padding:10px;
    margin:5px;
    border: 1px solid #ccc;
}
</style>