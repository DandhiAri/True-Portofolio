<template>
    <section class="h-screen bg-gray-100 flex flex-col justify-center items-center text-2xl font-bold text-gray-800">
        <p>{{ name  }}</p>
        <p>{{ title  }}</p>
    </section>
</template>

<script setup lang="ts">
interface Props {
    name:string;
    title:string;
}

withDefaults(defineProps<Props>(), {
    name: 'Dandhi Dwi Ari Prasetya',
    title: 'WEB DEVELOPER'
});

</script>