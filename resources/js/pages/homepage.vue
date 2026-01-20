<template>
    <portofoliolayout>
        <Head title="Portofolio home"></Head>
        <Herobanner :name="portofolioData.name" :title="portofolioData.title" />


    </portofoliolayout>
</template>
<script setup lang="ts">
import Herobanner from './portofolio/homepage/herobanner.vue';

const portofolioData = {
    name: 'Dandhi Dwi Ari Prasetya',
    title: 'WEB DEVELOPER'
};

</script>