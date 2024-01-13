<script>
    import Nav from './Nav.svelte'
    import TechBox from "./TechBox.svelte";
    import pilsopoly from '$lib/images/pilsopoly.svg';
    import fitBuddy from '$lib/images/fitbuddy.svg';
    import spaceGaze from '$lib/images/spacegaze.svg'
    import swagger from '$lib/images/swagger.svg'
</script>


<div id="main_page">
    <div class="column" id="first">
        <div>
            <h1>Robin Monseré</h1>
            <h2>Computer Science student</h2>
            <p>Interested in automation, efficient code and spaceflight.</p>
            <Nav></Nav>
        </div>
        <div id="contact" >
            <a href="https://www.linkedin.com/in/robin-monser%C3%A9/" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
            <a href="https://github.com/robinmonsere" target="_blank"><i class="fa-brands fa-github"></i></a>
            <a href="mailto: monsere.robin@gmail.com"><i class="fa-solid fa-envelope"></i></a>
        </div>
    </div>
    <div class="column" id="second">
        <div id="about">
            <p>I'm a 20-year-old <em>software engineering student</em> at Howest. I love building <em>automated systems</em> for the web and industries.
                Next to my studies and software, my interest lay with spaceflight and I actively contribute to a youth movement.</p>
            <br><p>In 2023 I went on a international study to the USA, and in 2024 I am doing an internship in mobile app development.</p>
        </div>
        <div id="skills">
            <p>My growing skillset includes</p>
            <h3>Mobile Development</h3>
            <div class="skills">
                <ul>
                    <li><svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>Kotlin</title><path d="M24 24H0V0h24L12 12Z"/></svg></li>
                    <li><svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>Flutter</title><path d="M14.314 0L2.3 12 6 15.7 21.684.013h-7.357zm.014 11.072L7.857 17.53l6.47 6.47H21.7l-6.46-6.468 6.46-6.46h-7.37z"/></svg></li>
                    <li><svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>Firebase</title><path d="M3.89 15.672L6.255.461A.542.542 0 017.27.288l2.543 4.771zm16.794 3.692l-2.25-14a.54.54 0 00-.919-.295L3.316 19.365l7.856 4.427a1.621 1.621 0 001.588 0zM14.3 7.147l-1.82-3.482a.542.542 0 00-.96 0L3.53 17.984z"/></svg></li>
                </ul>
            </div>
            <h3>Web Development</h3>
            <div class="skills">
                <ul>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                </ul>
                <img src="https://img.shields.io/badge/-0F172A?logo=html5&logoColor=white&style=for-the-badge" alt="HTML">
                <img src="https://img.shields.io/badge/-0F172A?logo=css3&logoColor=white&style=for-the-badge" alt="CSS">
                <img src="https://img.shields.io/badge/-0F172A?logo=sass&logoColor=white&style=for-the-badge" alt="SASS">
                <img src="https://img.shields.io/badge/-0F172A?logo=javascript&logoColor=white&style=for-the-badge" alt="JavaScript">
                <img src="https://img.shields.io/badge/-0F172A?logo=vue.js&logoColor=white&style=for-the-badge" alt="Vue.js">
                <img src="https://img.shields.io/badge/-0F172A?logo=node.js&logoColor=white&style=for-the-badge" alt="Node.js">
                <img src="https://img.shields.io/badge/-0F172A?logo=laravel&logoColor=white&style=for-the-badge" alt="Laravel">
            </div>

            <h3>Extra</h3>
            <div class="skills">
                 <ul>
                     <li><svg><svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>Swagger</title><path d="M12 0C5.383 0 0 5.383 0 12s5.383 12 12 12c6.616 0 12-5.383 12-12S18.616 0 12 0zm0 1.144c5.995 0 10.856 4.86 10.856 10.856 0 5.995-4.86 10.856-10.856 10.856-5.996 0-10.856-4.86-10.856-10.856C1.144 6.004 6.004 1.144 12 1.144zM8.37 5.868a6.707 6.707 0 0 0-.423.005c-.983.056-1.573.517-1.735 1.472-.115.665-.096 1.348-.143 2.017-.013.35-.05.697-.115 1.038-.134.609-.397.798-1.016.83a2.65 2.65 0 0 0-.244.042v1.463c1.126.055 1.278.452 1.37 1.629.033.429-.013.858.015 1.287.018.406.073.808.156 1.2.259 1.075 1.307 1.435 2.575 1.218v-1.283c-.203 0-.383.005-.558 0-.43-.013-.591-.12-.632-.535-.056-.535-.042-1.08-.075-1.62-.064-1.001-.175-1.988-1.153-2.625.503-.37.868-.812.983-1.398.083-.41.134-.821.166-1.237.028-.415-.023-.84.014-1.25.06-.665.102-.937.9-.91.12 0 .235-.017.369-.027v-1.31c-.16 0-.31-.004-.454-.006zm7.593.009a4.247 4.247 0 0 0-.813.06v1.274c.245 0 .434 0 .623.005.328.004.577.13.61.494.032.332.031.669.064 1.006.065.669.101 1.347.217 2.007.102.544.475.95.941 1.283-.817.549-1.057 1.333-1.098 2.215-.023.604-.037 1.213-.069 1.822-.028.554-.222.734-.78.748-.157.004-.31.018-.484.028v1.305c.327 0 .627.019.927 0 .932-.055 1.495-.507 1.68-1.412.078-.498.124-1 .138-1.504.032-.461.028-.927.074-1.384.069-.715.397-1.01 1.112-1.057a.972.972 0 0 0 .199-.046v-1.463c-.12-.014-.204-.027-.291-.032-.536-.023-.804-.203-.937-.71a5.146 5.146 0 0 1-.152-.993c-.037-.618-.033-1.241-.074-1.86-.08-1.192-.794-1.753-1.887-1.786zm-6.89 5.28a.844.844 0 0 0-.083 1.684h.055a.83.83 0 0 0 .877-.78v-.046a.845.845 0 0 0-.83-.858zm2.911 0a.808.808 0 0 0-.834.78c0 .027 0 .05.004.078 0 .503.342.826.859.826.507 0 .826-.332.826-.853-.005-.503-.342-.836-.855-.831zm2.963 0a.861.861 0 0 0-.876.835c0 .47.378.849.849.849h.009c.425.074.853-.337.881-.83.023-.457-.392-.854-.863-.854z"/></svg></svg></li>
                     <li></li>
                     <li></li>
                     <li></li>
                 </ul>
                <img src="https://img.shields.io/badge/-0F172A?logo=swagger&logoColor=white&style=for-the-badge" alt="Swagger">
                <img src="https://img.shields.io/badge/-0F172A?logo=postman&logoColor=white&style=for-the-badge" alt="postman">
                <img src="https://img.shields.io/badge/-0F172A?logo=docker&logoColor=white&style=for-the-badge" alt="Docker">
                <img src="https://img.shields.io/badge/-0F172A?logo=git&logoColor=white&style=for-the-badge" alt="Git">
            </div>
            <h3>Databases</h3>
            <div class="skills">
                <ul>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                </ul>
                <img src="https://img.shields.io/badge/-0F172A?logo=microsoft-sql-server&logoColor=white&style=for-the-badge"
                    alt="Microsoft SQL Server">
                <img src="https://img.shields.io/badge/-0F172A?logo=mongodb&logoColor=white&style=for-the-badge"
                     alt="MongoDB">
                <img src="https://img.shields.io/badge/-0F172A?logo=mysql&logoColor=white&style=for-the-badge"
                     alt="MySQL">
                <img src="https://img.shields.io/badge/-0F172A?logo=neo4j&logoColor=white&style=for-the-badge"
                     alt="Neo4j"></div>
            <h3>Operating Systems</h3>
            <div class="skills">
                <img src="https://img.shields.io/badge/-0F172A?logo=linux&logoColor=white&style=for-the-badge" alt="Linux">
                <img src="https://img.shields.io/badge/-0F172A?logo=windows&logoColor=white&style=for-the-badge" alt="Windows">
            </div>
            <h3>Other</h3>
            <div class="skills">
                <img src="https://img.shields.io/badge/-0F172A?logo=openjdk&logoColor=white&style=for-the-badge" alt="Java">
                <img src="https://img.shields.io/badge/-0F172A?logo=python&logoColor=white&style=for-the-badge" alt="Python">
                <img src="https://img.shields.io/badge/-0F172A?logo=.net&logoColor=white&style=for-the-badge" alt=".NET">
            </div>

        </div>
        <div id="projects">
            <div class="project">
                <div class="project_links">
                    <img src="{pilsopoly}" alt="pilsopoly logo">
                    <div class="source">
                        <a href="https://github.com/LukasOlivier/PilsoPoly-client" target="_blank"><i class="fa-solid fa-link"></i>Client</a>
                        <a href="https://github.com/LukasOlivier/PilsoPoly-server" target="_blank"><i class="fa-solid fa-link"></i>Server</a>
                    </div>
                </div>
                <div>
                    <h3>PilsoPoly - Web based Monopoly</h3>
                    <p>PilsoPoly, a game based on the popular Monopoly, is a functional, browser-playable Monopoly game with a special touch.</p><br>
                    <p>The client is built using standard HTML, CSS, and JavaScript, while the server is developed with Java (VertX) and utilizes a RESTful API.</p>
                    <br><p>PilsoPoly was designed and built by 4 students at Howest</p>

                    <div class="technologies">
                        <TechBox name="HTML5"/>
                        <TechBox name="CSS3"/>
                        <TechBox name="JavaScript"/>
                        <TechBox name="VertX"/>
                        <TechBox name="Proxmox"/>
                    </div>
                </div>
            </div>
            <div class="project">
                <div>
                    <img src="{fitBuddy}" alt="fitBuddy logo">

                </div>
                <div>
                    <h3>Fitness App “FitBuddy”</h3>
                    <p>I was part of a team of five students that developed a social media fitness app where users can track and share their workouts with friends.</p><br>
                    <p>I created a recommendation system through advanced filtering and machine learning.</p>
                    <div class="technologies">
                        <TechBox name="Flutter"/>
                        <TechBox name="Firebase"/>
                    </div>
                </div>
            </div>
            <div class="project">
                <div class="project_links">
                    <img src="{spaceGaze}" alt="spaceGaze logo">
                    <div class="source">
                        <a href="https://github.com/robinmonsere/SpaceGaze-Android-Only" target="_blank"><i class="fa-solid fa-link"></i>Source</a>
                    </div>

                </div>
                <div>
                    <h3>PilsoPoly - Web based Monopoly</h3>
                    <p>Developed an Android app using JetPack Compose to track the latest and upcoming rocket launches. Built on the public API of 'https://thespacedevs.com/' to display the most recent and up-to-date information on space exploration.</p><br>
                    <p>Planning to recreate this app in Flutter for IOS users.</p>
                    <div class="technologies">
                        <TechBox name="Kotlin"/>
                        <TechBox name="JetPack Compose"/>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>



<style>
    #main_page {
        display: flex;
        flex-direction: row;
        margin: 0 15vw 5rem 15vw;
        height: 100%;

    }

    #first {
        height: 80vh ;
        position: sticky;
        top: 5rem;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

    .column {
        width: 50%;
    }

    #second {
        overflow: clip;
    }

    h1 {
        font-weight: bold;
        font-size: 3.5rem;
    }

    h2 {
        margin: 0.8rem 0 0.8rem 0;
        font-size: 2rem;
    }

    h3 {
        font-weight: bold;
    }

    .project_links {
        display: flex;
        gap: 1rem;
        flex-direction: column;
        justify-content: space-between;
        color: var(--color-text-2);
    }

    .source {
        display: flex;
        flex-direction: column;
    }

    .project_links a {
        margin-top: 0.5rem;
        text-decoration: none;
        color: var(--color-text-2);
    }

    .project_links a i {
        margin-right: 0.5rem;
    }

    .project_links a:hover {
        color: var(--color-text);
    }

    #contact i {
        margin-right: 0.5rem;
        font-size: 1.8rem;
        color: lightgrey;
    }

    #contact i:hover {
        color: white;
        cursor: pointer;
    }

    p {
        line-height: 1.6rem;
        color: var(--color-text-2);
    }

    em {
        font-weight: bold;
        color: var(--color-text)
    }

    #about {
        padding-top: 5rem;
        margin: 0 1rem 3rem 1rem;
    }

    #skills {
        margin: 0 0 3rem 1rem;
    }

    #skills ul {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        gap: 1rem;
    }

    #skills li:hover svg {
        fill: var(--color-theme-1);
        cursor: pointer;
    }

    svg {
        width: 3rem;
        height: 3rem;
        fill: var(--color-text)
    }


    .project {
        display: flex;
        gap: 1rem;
        flex-direction: row;
        padding: 1rem;
        margin-right: 2px;
        border-radius: 0.5rem;
        margin-top: 1rem;
    }

    .project img {
        color: white;
        width: 5rem;
    }

    .project:hover {
        background: #121d34;
        box-shadow: 2px 3px #0a1b26;
    }

    .project:hover h3 {
        color: var(--color-theme-1);
    }

    .technologies {
        margin-top: 0.5rem;
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        gap: 0.5rem;
    }


    
</style>