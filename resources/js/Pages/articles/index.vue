<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
defineProps({ articles: Array })
</script>

<template>

    <Head title="Articoli" />

    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">Articoli</h2>
        </template>

        <div class="container mx-auto px-4">
            <div class="row">
                <div class="col">
                    <ul>
                        <li v-for="article in articles" :key="article.id">
                            <span>{{ article.name }} | </span>
                            <span>{{ article.url }}</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </AuthenticatedLayout>
</template>

<style>

</style>
