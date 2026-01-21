<template>
    <portofoliolayout>
        <Head title="Portofolio home"></Head>
        <Herobanner :name="portofolioData.name" :title="portofolioData.title" />
        <Contactinfo :email="portofolioData.email" :phone="portofolioData.phone" :github="portofolioData.github"/>

        <Contactsection />

    </portofoliolayout>
</template>
<script setup lang="ts">
import Contactinfo from './portofolio/homepage/contactinfo.vue';
import Contactsection from './portofolio/homepage/contactsection.vue';
import Herobanner from './portofolio/homepage/herobanner.vue';

const portofolioData = {
    name: 'Dandhi Dwi Ari Prasetya',
    title: 'WEB DEVELOPER',
    email: 'dandhiari@gmail.com',
    contact :{
        phone: '+62 8214 1794 129',
        github: 'https://github.com/DandhiAri'
    }
};

</script>