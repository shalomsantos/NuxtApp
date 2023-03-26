<template>
    <header class="container mx-auto p-4 flex justify-between shadow-sm bg-white">
        <Nav>
            <NuxtLink to="/produtos">nuxt dojo merch</NuxtLink>
        </Nav>
    </header>
    <div class="container mx-auto p-4">
        <slot/>
    </div>
    <footer class="container mx-auto p-4 flex justify-between shadow-sm bg-white">
        <ul class="flex gap-4">
            <li><NuxtLink class="font-bold" to="/">home</NuxtLink></li>
            <li><NuxtLink class="font-bold" to="/about">about</NuxtLink></li>
            <li><NuxtLink class="font-bold btn" to="/produtos">produtos</NuxtLink></li>
        </ul>
    </footer>
</template>

<script setup>
definePageMeta({
    layout: 'produtos'
})
</script>

<style scoped>
.router-link-exact-active{
    color: #12b488;
}
</style>