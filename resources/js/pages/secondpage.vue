<template>
    <div class="relative">
        <div class="relative">
            <Herobanner :name="portofolioData.name" :title="portofolioData.title" />
        </div>
        <Contactinfo :email="portofolioData.contactinfo.email" :github="portofolioData.contactinfo.github" />
        <Biography :content="portofolioData.biography.content"  :tools="portofolioData.biography.tools"/>
        <section class="relative p-10">
            <div class="absolute -inset-1 bg-repeat-round opacity-30 bg-[url(/img/4ktopo.jpg)]"></div>

            <div class="absolute -inset-1 bg-gradient-to-b from-black via-black/50 to-transparent pointer-events-none"></div>
            <Projectsection class="relative z-999" :title="portofolioData.projects.title" :quote="portofolioData.projects.quote" :projects="portofolioData.projects.project"/>
        </section>
        <Footer :copyright="portofolioData.footer" />
    </div>
</template>
<script setup>
    import Herobanner from './portofolio/homepage/herobanner.vue';
    import Contactinfo from './portofolio/homepage/contactinfo.vue';
    import Biography from './portofolio/homepage/biography.vue';
    import Projectsection from './portofolio/homepage/projectsection.vue';
    import Footer from './portofolio/homepage/footer.vue';

    const portofolioData = {
        name: 'Dandhi Dwi Ari Prasetya',
        title: 'WEB DEVELOPER | COMPUTER ENGINEER | IOT ENGINEER',
        contactinfo: {
            email: 'dandhiari@gmail.com',
            github: 'https://github.com/DandhiAri'
        },
        biography: {
            content: "HIII :D NICE TO MEET YOUU, Im a Computer Engineering fresh graduate (GPA 3.77) with a core foundation in software engineering. My technical focus spans End-to-End Web Development & IoT Integration, blending full-stack coding capabilities (frontend/backend) with hands-on network infrastructure configuration and hardware management. Currently, I am engineering a full-stack e-commerce platform for an export startup and developing several personal projects, including retail web platforms and a modern portfolio. I am looking for more experience and interested in working with projects and jobs that are relevant to the fields below:",
            tools: [
                { name: 'Web Development', icon: 'img/tools/html.png' },
                { name: 'IT Support', icon: 'img/tools/css.png' },
                { name: 'Networking', icon: 'img/tools/javascript.png' },
                { name: 'Frontend Development', icon: 'img/tools/vue.png' },
                { name: 'Laravel', icon: 'img/tools/laravel.png' },
                { name: 'Node.js', icon: 'img/tools/nodejs.png' },
                { name: 'Python', icon: 'img/tools/python.png' },
                { name: 'Docker', icon: 'img/tools/docker.png' },
                { name: 'Git', icon: 'img/tools/git.png' },
                { name: 'HTML', icon: 'img/tools/html.png' },
                { name: 'CSS', icon: 'img/tools/css.png' },
                { name: 'JavaScript', icon: 'img/tools/javascript.png' },
                { name: 'Vue.js', icon: 'img/tools/vue.png' },
                { name: 'Laravel', icon: 'img/tools/laravel.png' },
                { name: 'Node.js', icon: 'img/tools/nodejs.png' },
                { name: 'Python', icon: 'img/tools/python.png' },
                { name: 'Docker', icon: 'img/tools/docker.png' },
                { name: 'Git', icon: 'img/tools/git.png' },
                { name: 'Laravel', icon: 'img/tools/laravel.png' },
                { name: 'Node.js', icon: 'img/tools/nodejs.png' },
                { name: 'Python', icon: 'img/tools/python.png' },
                { name: 'Docker', icon: 'img/tools/docker.png' },
                { name: 'Git', icon: 'img/tools/git.png' },
            ]
        },
        projects:{
            title:"Projects",
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
        footer:"Copyright &copy; 2026 Dandhi Dwi Ari Prasetya. All rights reserved.",
        
    }
</script>
<style scoped>
    .body-content{
        margin: 0 5%;
    }
    body{
        -webkit-overflow-scrolling: touch;
    }
</style>