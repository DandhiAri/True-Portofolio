<template>
    <!-- <Herobanner :name="portofolioData.name" :title="portofolioData.title" /> -->
    <Contactinfo :email="portofolioData.contactinfo.email" />
    <Projectsection :title="portofolioData.project.title" :quote="portofolioData.project.quote" :projects="portofolioData.project.projects"/>
    <!-- <Contactsection :quotes="portofolioData.quotes" /> -->
</template>
<script setup>
    import Contactinfo from './portofolio/homepage/contactinfo.vue';
    import Contactsection from './portofolio/homepage/contactsection.vue';
    import Herobanner from './portofolio/homepage/herobanner.vue';
    import Projectsection from './portofolio/homepage/projectsection.vue';

    const portofolioData = {
        name: 'Dandhi Dwi Ari Prasetya',
        title: 'WEB DEVELOPER',
        contactinfo: {
            email: 'dandhiari (at) gmail [dot] com'
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
    }
</script>   