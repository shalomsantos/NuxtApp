<template>
    <header class="shadow-sm bg-white">
        <nav class="container mx-auto p-4 flex justify-between ">
            <NuxtLink class="font-bold" to="/">nuxt dojo</NuxtLink>
            <ul class="flex gap-4">
                <li><NuxtLink class="font-bold" to="/">home</NuxtLink></li>
                <li><NuxtLink class="font-bold" to="/about">about</NuxtLink></li>
                <li><NuxtLink class="font-bold btn" to="/produtos">produtos</NuxtLink></li>
            </ul>
            <a href="/about">Normal link -- about page</a>
        </nav>
    </header>
    <div class="container mx-auto p-4">
        <slot/>
    </div>
</template>

<style scoped>
.router-link-exact-active{
    color: #12b488;
}
</style>