<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
import { Link } from '@inertiajs/vue3';

defineProps({
    id: Number,
    article: Object
})
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
                    <form >

                    </form>
                </div>
            </div>
        </div>
    </AuthenticatedLayout>
</template>

<style>

</style>
