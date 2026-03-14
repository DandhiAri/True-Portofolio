<template>
    <div class="relative bg-black">
        <div class="relative">
            <Herobanner :name="portofolioData.name" :title="portofolioData.title" />
        </div>

        <Contactinfo :email="portofolioData.contactinfo.email" />
        <section class="body-content py-10">
            <Projectsection :title="portofolioData.projects.title" :quote="portofolioData.projects.quote" :projects="portofolioData.projects.project"/>
        </section>
    </div>
</template>
<script setup>
    import Herobanner from './portofolio/homepage/herobanner.vue';
    import Contactinfo from './portofolio/homepage/contactinfo.vue';
    import Projectsection from './portofolio/homepage/projectsection.vue';
    
    const portofolioData = {
        name: 'Dandhi Dwi Ari Prasetya',
        title: 'WEB DEVELOPER | NETWORK ENGINEER | IOT ENGINEER',
        contactinfo: {
            email: 'dandhiari@gmail.com '
        },
        projects:{
            title:"My Work So far... and yet still CONTINUE !",
            // quote:"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos necessitatibus numquam quo sit distinctio nisi, exercitationem officia.",
            project:[
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
            ]
        },
    }
</script>
<style scoped>
    .body-content{
        margin: 0 5%;
    }
</style>