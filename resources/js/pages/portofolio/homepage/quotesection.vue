<template>
    <section class="flex justify-between">
        <div v-for="quote in quotes" :key="quote.position" :class="quote.position === 'left' ? 'max-w-fit' : 'text-fit max-w-xs text-gray-600'">
            <div class="text-lg" v-if="quote.position === 'left'">
                {{ quote.text }}<br />
                {{ quote.translation }}<br />
                <p>{{ quote.source }}</p>
            </div>
            <div v-else>
                <p class="text-xs">{{ quote.text }}</p>
                <p class="text-black font-bold text-lg mt-2">{{ quote.link }}</p>
            </div>
        </div>
    </section>
</template>
<script setup lang="ts">
interface Quote {
    position: string;
    text: string;
    translation?: string;
    source?: string;
    link?: string;
}

interface Props {
    quotes: Quote[];
}

defineProps<Props>();
</script>