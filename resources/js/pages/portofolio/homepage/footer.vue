<template>
    <footer>
        <p>{{ copyright }}</p>
    </footer>
</template>
<script setup lang="ts">
    interface Props{
        copyright:string;
    }
    defineProps<Props>();
</script>