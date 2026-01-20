<template>
    <div class="m-4">
        <img class="w-96 rounded-3xl p-0" 
        :src="image" 
        :alt="title" 
        />
        <p class="text-left text-xl mt-2">{{ title }}</p>
    </div>
</template>
<script setup lang ="ts">
    interface Props{
        image: string;
        title: string;
    }
    defineProps<Props>();
</script>