<template>
    <section class=" my-10">
        <div class="text-4xl font-bold flex justify-between">
            {{ title }}
            <p class="text-xs font-normal text-fit text-gray-600 max-w-xs">
                {{ quote }}
            </p>
        </div>
        <div class="mt-3 gap-4 flex flex-wrap justify-center">
            <div v-for="project in projects" class="max-w-md m-1">
                <img class="w-150 rounded-xl" :src="project.imgproject" :alt="project.nameproject" srcset="">
                <p class="text-2xl mt-2"> {{ project.nameproject }}</p>
                <p class="text-gray-600 text-justify">Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis adipisci eaque consequuntur earum expedita nulla mollitia porro magnam ducimus sit, molestias facere soluta possimus aperiam doloribus itaque eum corrupti quod.</p>
                <div class="flex flex-wrap mt-2 gap-2">
                    <p class="text-sm m-1">Laravel</p> 
                    <p class="text-sm m-1">Laravel</p>  
                    <p class="text-sm m-1">Laravel</p> 
                    <p class="text-sm m-1">Laravel</p> 
                </div>
            </div>
        </div>
    </section>
</template>
<script setup lang="ts">
interface Project{
    imgproject:string;
    nameproject:string;
    // description:string;
}

interface Props{
    title:string;
    quote:string;
    projects:Project[];
}

defineProps<Props>();
</script>