<template>
    <div class="h-screen flex justify-center items-center">
        <div class="mt-7 h-fit max-w-sm px-14 text-center card">
            <p class="mt-7 text-7xl font-bold text-green-600">{{ error.statusCode }}</p>
            <p class="mt-7 text-4xl">Ooops.</p>
            <p class="mt-7">{{ error.message }}</p>
            <button class="btn my-7" @click="handleClearError">Go Home...</button>
        </div>
    </div>

</template>

<script setup>
defineProps(['error'])

const handleClearError = () => clearError({ redirect: '/'})

</script>

<style scoped></style>