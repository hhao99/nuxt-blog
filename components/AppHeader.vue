<template>
    <div class="flex flex-row bg-gray-200 min-w-screen p-4">
        <h1 class="text-3xl min-w-[75%] text-center">NUXT World</h1>
        <nav class="shadow-lg bg-gray-300 p-4 rounded-lg">
            <ul class="flex flex-row space-x-4">
                <li v-for="link in links" :key="link.url">
                    <nuxt-link :to="link.url">{{ link.name }}</nuxt-link>
                </li>
            </ul>
        </nav>        
    </div>
</template>

<script lang="ts" setup>
    const links = [
        { name: 'Home', url: '/' },
        { name: 'About', url: '/about' },
        { name: 'Contact', url: '/contact' },
    ];
</script>