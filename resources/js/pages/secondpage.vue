<template>
    <Herobanner :name="portofolioData.name" :title="portofolioData.title" />
    <Contactinfo :email="portofolioData.contactinfo.email" />
    <Projectsection :title="portofolioData.project.title" :quote="portofolioData.project.quote" :projects="portofolioData.project.projects"/>
    <!-- <Contactsection :quotes="portofolioData.quotes" /> -->
</template>
<script setup>
    import Herobanner from './portofolio/homepage/herobanner.vue';
    import Contactinfo from './portofolio/homepage/contactinfo.vue';
    import Projectsection from './portofolio/homepage/projectsection.vue';

    const portofolioData = {
        name: 'Dandhi Dwi Ari Prasetya',
        title: 'WEB DEVELOPER',
        contactinfo: {
            email: 'dandhiari@gmail.com '
        },
        project:{
            title:"My Work So far... and yet still continue!",
            // quote:"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos necessitatibus numquam quo sit distinctio nisi, exercitationem officia.",
            projects:[
                {
                    imgproject:"img/projects/dummy.png",
                    nameproject:"INIT (Inventory IT)"
                },
                {
                    imgproject:"img/projects/dummy.png",
                    nameproject:"DFOOD"
                },
                {
                    imgproject:"img/projects/dummy.png",
                    nameproject:"Art Of Manunggalan 9.0"
                },            
                // {
                //     imgproject:"img/projects/dummy.png",
                //     nameproject:"Landing Page of Nusantara Tama"
                // },
            ]
        },
    }
</script>   