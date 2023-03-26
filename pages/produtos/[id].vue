<template>
    <div>
        <p>{{ produto.title }}</p>
        <p>{{ produto.price }}</p>
        <p>{{ produto.id }}</p>
    </div>
</template>

<script setup>
const { id } = useRoute().params
const url = 'https://fakestoreapi.com/products/' + id

const { data: produto } =  await useFetch(url)

definePageMeta({
    layout: 'produtos'
})
</script>

<style scoped>

</style>