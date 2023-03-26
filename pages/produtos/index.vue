<template>
    <div>
       <div class="grid grid-cols-4 gap-5">
            <div v-for="p in produtos">
                <NuxtLink :to="`/produtos/${p.id}`">{{ p.title }}</NuxtLink>
            </div>
       </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: 'produtos'
})
const { data: produtos } =  await useFetch('https://fakestoreapi.com/products')
</script>

<style scoped>

</style>