<template>
    <section class="items-center justify-center bg-gray-100 py-10 font-bold">
        <div class="px-4 text-center">
            <h1
                class="text-4xl tracking-tighter text-black uppercase md:text-6xl"
            >
                {{ name }}
            </h1>
            <p class="mt-4 text-xl tracking-widest text-gray-500">
                {{ title }}
            </p>
        </div>
    </section>
</template>

<script setup>
defineProps(['name', 'title']);
</script>