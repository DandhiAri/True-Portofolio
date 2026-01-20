<template>
    <Head title="Portofolio Home" />
    <!-- <div class="navbar">
        <nav>
            <ul class="nav-links">
                <li><a href="/about">About</a></li>
                <li><a href="/projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </div> -->
    <div class="herobanner">
        <p>Dandhi Dwi Ari Prasetya</p></br>
        <p>WEB DEVELOPER</p>
    </div>
    <div class="contact-info">
        <p>Email: dandhiari@gmail.com | Phone: +62 821 4179 4129 | Github: <a href="https://github.com/DandhiAri">DandhiAri</a></p>
    </div>

    <section class="body">
        <section class="quote-line">
            <div class="left-quote">
                「雨が降っても　花は咲くから　前を向いて」<br>
                "Even if it rains, flowers will still bloom, so keep looking forward."<br>
                <p class="">-"lilac" by Mrs. Green Apple</p>
            </div>
            <div class="right-quote">
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.
                    Lorem ipsum dolor, sit amet consectetur adipisicing elit.
                </p>
                <p class="link-about">More about me!</p>
            </div>
        </section>
        <section class="my-projects">
            <div class="sub-section-title space-between">
                My Work So far... and yet still continue!
                <p class="right-quote">
                    Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos necessitatibus numquam quo sit distinctio nisi, exercitationem officia.
                </p>
            </div>
            <div class="project-body">
                <div class="project-container">
                    <img class="img-project" src="img/projects/dummy.png" alt="project-img" srcset="">
                    <p>project name &#62;&#62;&#62;</p>
                </div>
                <div class="project-container">
                    <img class="img-project" src="img/projects/dummy.png" alt="project-img" srcset="">
                    <p>project name &#62;&#62;&#62;</p>
                </div>
                <div class="project-container">
                    <img class="img-project" src="img/projects/dummy.png" alt="project-img" srcset="">
                    <p>project name &#62;&#62;&#62;</p>
                </div>
                <div class="project-container">
                    <img class="img-project" src="img/projects/dummy.png" alt="project-img" srcset="">
                    <p>project name &#62;&#62;&#62;</p>
                </div> 
            </div>
        </section>
        <section class="contact-us">
            <div class="sub-section-title">
                Have a project idea? <strong>Let's Work Together!</strong><br>
                Or maybe just saying hi&#8230; 
                <span style="text-decoration: underline;">Let's talk!</span>
                <hr class="line-on-contact">
            </div>
            <div class="btn-contact">
                Contact Me!
            </div>
            <div class="contact-context">

                <p>
                    <div class="sml-context">Email:</div>
                    dandhiari@gmail.com
                </p>
                <p>
                    <div class="sml-context">Phone:</div>
                    +62 821 4179 4129
                </p>
            </div>
            <form action="" method="post">
                <input type="text" name="subject" id="">
                <input type="text" name="content" id="">
                <input type="submit" value="">
            </form>
        </section>
    </section>
    <footer>
        <p>&copy; 2026 Dandhi Dwi Ari Prasetya. All rights reserved.</p>
    </footer>
</template>

<style>
.space-between{
    display: flex;
    justify-content: space-between;
}
body{
    background-color: #f4f4f4;
    color: black;
}
section {
    margin: 2em;
}
.body{
    margin: 3em;
}
.sub-section-title {
    font-size: 2em;
    font-weight: bold;
}
.quote-line{
    display:flex;
    justify-content: space-between;
    /* grid-template-columns: ; */
}
.right-quote {
    font-size: 12px;
    max-width: 25%;
    /* font-style: italic; */
    color:#333;
    font-weight: normal;
}

.link-about{
    color:black;
    font-weight: bold;
    font-size: 1.2em;
    margin-top:10px;
}
.project-body {
    /* padding: 1em 0 0 0; */
    display: flex;
    gap: 1em;
    flex-wrap: wrap;
    justify-content: start;
    justify-content: center;
}
.project-container{
    margin:1em;
}
.img-project {
    padding: 0em;
    width: 35em;
    border-radius: 30px;
}
.project-container p {
    text-align: left;
    font-size: 1.5em;
    /* font-weight: bold; */
    margin-top: 0.5em;
}

.navbar {
    background-color: #333;
    padding: 1rem;
    display: flex;
    justify-content: center;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 1rem;
}

.nav-links li a {
    color: white;
}

.herobanner {
    height: 80vh;
    background-color: #f4f4f4;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-size: 2rem;
    font-weight: bold;
    color: #333;
}
.contact-us {
    /* text-align: center; */
    display: grid;
    grid-template-columns: 80% 20%;
    margin-top: 4em;
}
/* .contact-us:nth-child(2) {
    grid-row: 2 span;
    text-align: center;
} */
.contact-context {
    margin-top: 0em;
    font-size: 15px;
    display: flex;
    color:#333;
}
.contact-context .sml-context {
    font-weight: bold;
    display: block;
    margin-right: 0.5em;
    font-size: small;
    
}
.contact-context p {
    margin-right: 2em;
}
.contact-info {
    background-color: #333;
    color: white;
    margin: auto;
    display: grid;
    text-align: center;
    align-content: center;
    padding: 0.5rem;
    height: 10vh;
}
.contact-info p a{
    text-decoration: underline;
}
.line-on-contact{
    margin-top:20px;    
}

.btn-contact {
    margin: 1em;
    padding: 3em 1em;
    font-weight: bold;
    background-color: blue;
    font-size: 1.3em;
    color: white;
    text-align: center;
    /* display: flex; */
    /* justify-content: center; */
    /* align-content: center; */
    align-items: center;
    min-width: 3em;
    /* width: fit-content; */
    flex-wrap:wrap;
    border-radius: 10px;
    cursor: pointer;
    grid-row: span 2;
}

footer {
    text-align: center;
    background-color: black;
    color: white;
}
</style>