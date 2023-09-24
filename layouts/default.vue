<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <NuxtLink to="/" class="font-bold">Demo Shop</NuxtLink>
                <ul class="flex gap-4">
                    <li><Nuxt-link to="/">Home</Nuxt-link></li>
                    <li><Nuxt-link to="/about">About</Nuxt-link></li>
                    <li><Nuxt-link to="/products">Products</Nuxt-link></li>
                </ul>
            </nav>
        </header>
    </div>
    <div class="container mx-auto p-4">
        <slot />
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
.router-link-exact-active {
    color: rgb(92, 189, 149)
}
</style>