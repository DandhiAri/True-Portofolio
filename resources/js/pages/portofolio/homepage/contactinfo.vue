<template>
    <div class="bg-neutral-900 p-5 grid content-center text-white text-center h-15">
        <p class="flex justify-center"> <div class="underline mr-1"> Email:  {{email}} </div> | <div v-show="phone"> Phone: {{phone}} |</div><a class="underline ml-1" href="{{ github }}">Github: @DandhiAri</a></p>
    </div>
</template>
<script setup lang="ts">
    interface Props{
        email:string;
        phone?:string;   
        github:string;
    }
    defineProps<Props>();
</script>
