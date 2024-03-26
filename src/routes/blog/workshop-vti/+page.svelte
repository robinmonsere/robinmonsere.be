<script>
    import workshop1 from "../images/workshop1.jpg";
    import workshop2 from "../images/workshop2.jpg";
    import workshop3 from "../images/workshop3.jpg";
</script>

<a id="backButton" href="/blog"><i class="fa-solid fa-arrow-left"></i> Go back</a>
<h1>Workshop @ VTI Izegem</h1>

<p>
    Together with <a id="person" href="">Sibren Eeckhout</a>, <a id="person" href="https://lukasolivier.be/">Lukas Olivier</a>,
    <a id="person" href="https://nielssoete.be/">Niels Soete</a>,
    <a id="person" href="https://www.linkedin.com/in/lucas-guillemyn-280103g/">Lucas Guillemyn</a> and
    <a id="person" href="https://www.thiboverbeerst.com/">Thibo Verbeerst</a>, I created and participated in a workshop at VTI Izegem.
</p>
<p>Our goal was to educate students at VTI Izegem on what things we learn at Howest.</p>
<h2>Flask API</h2>
<p>With the help of template code and the whole team answering questions, the students were able to create a Flask API that could add, receive or generate random quotes.</p>
<p>Students learned the importance of client/server architecture, and the communication between the frontend and backend </p>

<h2>Pentesting</h2>
<p>For the purpose of this workshop, we created a fake banking website. This website would be the playground where the students could try out all different kind of pentesting tasks</p>
<p>With help from the team, the students were able to use OSINT techniques to find the password of the fake bank manager and login to his account. After successfully doing so, they could abuse the developer tools and change the salary of an employee. </p>

<h2>Special Thanks to VTI Izegem!</h2>
<p>As a team, we thank the lecturers at VTI Izegem to allow us to teach to their students.</p>

<p>You can try the workshop for yourself <a id="person" href="https://drive.google.com/drive/folders/1YFTZ3GLQilWwrtiMukJCJgMazEaH1Dec">here.</a></p>

<div id="images">
    <img src="{workshop1}" alt="">
    <img src="{workshop2}" alt="">
    <img src="{workshop3}" alt="">
</div>

<style>

    #images {
        padding-top: 5rem;
        display: flex;
        flex-wrap: wrap;
        gap: 5rem;
    }
    img {
        width: 40%;
        height: 30rem;
        margin-bottom: 1rem;
        object-fit: cover;
    }

    #person {
        color: var(--color-theme-1);
        text-decoration: underline;
    }

    #backButton {
        display: flex;
        align-items: center;
        margin-bottom: 2rem;
        gap: 1rem;
    }
    i {
        font-size: 2rem;

    }

    h1 {

        color: var(--color-theme-1);
        font-size: 2.5rem;
        padding-bottom: 1rem;
    }
    h2 {
        font-weight: 700;
        font-size: 1.5rem;
        padding-bottom: 1rem;
        padding-top: 2rem;
    }
    p {
        color: var(--color-text-1);
        line-height: 1.5rem;
    }
</style>