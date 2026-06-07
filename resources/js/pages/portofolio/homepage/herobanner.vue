<template>
    <section class="items-center justify-center bg-cover bg-[url(/img/dandhinabila.png)] py-10 font-bold">
        <div class="px-4 text-center">
            <h1
                class="text-4xl tracking-tighter text-black uppercase md:text-6xl bg-white bg-opacity-50 p-2"
            >
                {{ name }}
            </h1>
            <p class="mt-4 text-xl tracking-widest text-white uppercase bg-black bg-opacity-50 p-1">
                {{ title }}
            </p>
        </div>
    </section>
</template>

<script setup>
defineProps(['name', 'title']);
</script>
