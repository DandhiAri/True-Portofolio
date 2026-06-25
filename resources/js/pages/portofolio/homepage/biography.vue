<template>
    <div class="bg-black relative p-10">
        <p class="text-lg text-gray-300 leading-relaxed">{{ content }}</p>
        <div class="flex flex-wrap justify-center gap-3 mt-6 mx-auto">
            <div class="text-xl font-bold text-zinc-300">Interested/Learning:</div>
            <div 
                v-for="tool in tools" 
                :key="tool.name" 
                class="transition-all duration-200 hover:-translate-y-0.5"
            >
                <span class="block rounded-full border border-zinc-800/80 bg-zinc-900/30 px-5 py-2 text-sm font-medium text-zinc-300 shadow-sm backdrop-blur-sm select-none">
                    {{ tool.name }}
                </span>
            </div>
        </div>
    </div>
</template>
<script setup lang="ts">
    interface Tool {
        name: string;
        icon: string;
    }

    interface Props {
        content: string;
        tools: Tool[];
    }

    defineProps<Props>();
</script>