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
        title: 'WEB DEVELOPER | NETWORK ENGINEER | IOT ENGINEER',
        contactinfo: {
            email: 'dandhiari@gmail.com',
            github: 'https://github.com/DandhiAri'
        },
        biography: {
            content: "Hello, I'm Dandhi Dwi Ari Prasetya, a passionate web developer and network engineer. I specialize in creating dynamic and responsive web applications, as well as designing and managing complex network infrastructures. With a strong foundation in both front-end and back-end development, I strive to deliver seamless user experiences and robust solutions. My expertise extends to IoT engineering, where I explore innovative ways to connect devices and enhance automation. I am committed to continuous learning and staying updated with the latest technologies to provide cutting-edge solutions.",
            tools: [
                { name: 'HTML', icon: 'img/tools/html.png' },
                { name: 'CSS', icon: 'img/tools/css.png' },
                { name: 'JavaScript', icon: 'img/tools/javascript.png' },
                { name: 'Vue.js', icon: 'img/tools/vue.png' },
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