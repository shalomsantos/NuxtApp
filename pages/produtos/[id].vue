<template>
    <div>
        <p class="font-bold">detalhes do produto: {{ id }}</p>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Fuga mollitia cumque ducimus, velit excepturi non corrupti 
            libero assumenda laboriosam, rem quia quisquam laborum suscipit voluptatum, labore dicta provident magnam sunt?</p>
    </div>
</template>

<script setup>
const { id } = useRoute().params
</script>

<style>

</style>