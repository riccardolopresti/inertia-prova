<script setup>
import AppHeader from '@/Pages/AppHeader.vue';
import { Head } from '@inertiajs/vue3';

defineProps({ articles: Array })
</script>

<template>
    <Head title="Articoli" />


    <AppHeader/>

    <div class="container mt-40 mx-auto">
        <ul>
            <li v-for="article in articles" :key="article.id">
                <span>{{ article.name }}  | </span>
                <span>{{ article.url }}</span>
            </li>
        </ul>
    </div>
</template>


<style>

</style>
