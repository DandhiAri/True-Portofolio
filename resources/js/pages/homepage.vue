<template>
    <portofoliolayout>
        <Head title="Portofolio home"></Head>
        <Herobanner :name="portofolioData.name" :title="portofolioData.title" />
        <Contactinfo :email="portofolioData.contactinfo.email" :phone="portofolioData.contactinfo.phone" :github="portofolioData.contactinfo.github"/>
        
        <section class="p-15">

            <Quotesection :quotes="portofolioData.quotes" /> 
            <!-- <Contactsection /> -->
            <Projectsection :projects="portofolioData.project.projects" :title="portofolioData.project.title" :quote="portofolioData.project.quote"/>

            <Contactsection :text="portofolioData.contactsection.text" :btn="portofolioData.contactsection.btn" :email="portofolioData.contactinfo.email" :phone="portofolioData.contactinfo.phone" />
        </section>

        <Footer :copyright="portofolioData.footer" />
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
import Footer from './portofolio/homepage/footer.vue';
import Herobanner from './portofolio/homepage/herobanner.vue';
import Projectsection from './portofolio/homepage/projectsection.vue';
import Quotesection from './portofolio/homepage/quotesection.vue';

const portofolioData = {
    name: 'Dandhi Dwi Ari Prasetya',
    title: 'WEB DEVELOPER',
    contactinfo: {
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
            text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit.Lorem ipsum dolor, sit amet consectetur adipisicing elit.',
            link: 'More about me!'
        }
    ],
    project:{
        title:"My Work So far... and yet still continue!",
        quote:"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos necessitatibus numquam quo sit distinctio nisi, exercitationem officia.",
        projects:[
            {
                imgproject:"img/projects/dummy.png",
                nameproject:"project name"
            },
            {
                imgproject:"img/projects/dummy.png",
                nameproject:"project name"
            },
            {
                imgproject:"img/projects/dummy.png",
                nameproject:"project name"
            },            
            {
                imgproject:"img/projects/dummy.png",
                nameproject:"project name"
            },
        ]
    },
    contactsection:{
        text:"Have a project idea? <strong>Let's Work Together!</strong><br>Or maybe just saying hi&#8230;<span class='underline'>Let's talk!</span>",
        btn:"Contact Us!",
    },
    footer: "&copy; 2026 Dandhi Dwi Ari Prasetya. All rights reserved.",
};

</script>