<template>
    <portofoliolayout>
        <Head title="Portofolio home"></Head>
        <Herobanner :name="portofolioData.name" :title="portofolioData.title" />
        <Contactinfo :email="portofolioData.contact.email" :phone="portofolioData.contact.phone" :github="portofolioData.contact.github"/>

        <Quotesection :quotes="portofolioData.quotes" /> 

        <Contactsection />

    </portofoliolayout>
</template>
<style>
    body{
        background-color: #fff;
        color: black;
    }
</style>
<script setup lang="ts">
import Contactinfo from './portofolio/homepage/contactinfo.vue';
import Contactsection from './portofolio/homepage/contactsection.vue';
import Herobanner from './portofolio/homepage/herobanner.vue';
import Quotesection from './portofolio/homepage/quotesection.vue';

const portofolioData = {
    name: 'Dandhi Dwi Ari Prasetya',
    title: 'WEB DEVELOPER',
    contact: {
        email: 'dandhiari@gmail.com',
        phone: '+62 8214 1794 129',
        github: 'https://github.com/DandhiAri'
    },
    quotes: [
        {
            position: 'left',
            text: '「雨が降っても　花は咲くから　前を向いて」',
            translation: '"Even if it rains, flowers will still bloom, so keep looking forward."',
            source: '-"lilac" by Mrs. Green Apple'
        },
        {
            position: 'right',
            text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Lorem ipsum dolor, sit amet consectetur adipisicing elit.',
            link: 'More about me!'
        }
    ]

        
};

</script>