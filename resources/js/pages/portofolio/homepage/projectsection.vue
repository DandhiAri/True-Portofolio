<template>
    <section class="mt-20">
        <div class="text-4xl font-bold flex justify-between">
            {{ title }}
            <p class="text-xs font-normal text-fit text-gray-600 max-w-xs">
                {{ quote }}
            </p>
        </div>
        <div class="mt-3 gap-4 flex flex-wrap justify-center">
            <div v-for="project in projects" class="m-1">
                <img class="w-150 rounded-xl" :src="project.imgproject" :alt="project.nameproject" srcset="">
                <p class="text-2xl mt-1"> {{ project.nameproject }} &#62;&#62;&#62;</p>
            </div>
        </div>
    </section>
</template>
<script setup lang="ts">
interface Project{
    imgproject:string;
    nameproject:string;
}

interface Props{
    title:string;
    quote:string;
    projects:Project[];
}

defineProps<Props>();
</script>