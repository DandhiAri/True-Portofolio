<template>
    <div class="bg-neutral-900 p-5 grid content-center text-white text-center h-15">
        <p>Email:  {{email}} | Phone:   {{phone}} | Github: <a class="underline" href="{{ github }}">DandhiAri</a></p>
    </div>
</template>
<script setup lang="ts">
    interface Props{
        email:string;
        phone:string;   
        github:string;
    }
    defineProps<Props>();
</script>
