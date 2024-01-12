<script>
    import Nav from './Nav.svelte'
    import TechBox from "./TechBox.svelte";
    import pilsopoly from '$lib/images/pilsopoly.svg';
    import fitBuddy from '$lib/images/fitbuddy.svg';
    import spaceGaze from '$lib/images/spacegaze.svg'
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
        height: 200vh;
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
        margin: 0 1rem 3rem 1rem;
        padding-top: 5rem;

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