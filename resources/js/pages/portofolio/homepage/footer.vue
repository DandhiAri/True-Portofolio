<template>
    <footer class="bg-black text-white p-1 text-center">
        <div v-html="copyright"></div>
    </footer>
</template>
<script setup lang="ts">
    interface Props{
        copyright:string;
    }
    defineProps<Props>();
</script>