<script>
    import usa1 from '$lib/images/usa (1).jpg';
    import usa2 from '$lib/images/usa (2).jpg';
    import usa3 from '$lib/images/usa (3).jpg';
    import usa4 from '$lib/images/usa (4).jpg';
    import usa5 from '$lib/images/usa (5).jpg';
    import usa6 from '$lib/images/usa (6).jpg';
    import usa7 from '$lib/images/usa (7).jpg';
    import usa8 from '$lib/images/usa (8).jpg';
    import usa9 from '$lib/images/usa (9).jpg';
    import usa10 from '$lib/images/usa (10).jpg';
    import usa11 from '$lib/images/usa (11).jpg';
    import usa12 from '$lib/images/usa (12).jpg';

</script>

<h1>International Study in the USA</h1>
<h2>Arrival in Texas Tyler</h2>
<p>In the second half of 2023, I had the opportunity to study in the United States. My journey took me to Texas Tyler, a vibrant and welcoming community that quickly became my home away from home. The experience of studying abroad was transformative, offering me new perspectives and enriching my understanding of different cultures and educational systems.</p>
<h2>Academic Excellence</h2>
<p>Texas Tyler provided a unique blend of academic rigor and southern hospitality. The university's diverse range of courses and highly qualified faculty ensured that I received a top-notch education. The campus was bustling with activities, and I found numerous opportunities to engage in extracurricular pursuits that complemented my studies. The support from both faculty and fellow students was invaluable, making the transition to a new academic environment smooth and enjoyable.</p>
<h2>Cultural Immersion</h2>
<p>Beyond the classroom, living in Tyler allowed me to immerse myself in the local culture. The city's rich history and dynamic community events offered endless opportunities for exploration and learning. From attending local festivals to visiting historical sites, I was able to gain a deeper appreciation for the unique Texan way of life. The friendships I made with locals and other international students added a personal dimension to my experience, making it even more memorable.</p>
<h2>A Lasting Impact</h2>
<p>Overall, my time in Texas Tyler was a defining chapter in my educational journey. The combination of high-quality education, cultural immersion, and the warmth of the local community made it an unforgettable experience. Studying abroad not only broadened my academic horizons but also enriched my personal growth, leaving me with cherished memories and a lasting connection to the United States.</p>
<div id="images">
    <img src="{usa2}" alt="">
    <img src="{usa1}" alt="">
    <img src="{usa12}" alt="">

    <img src="{usa4}" alt="">
    <img src="{usa6}" alt="">
    <img src="{usa7}" alt="">
    <img src="{usa8}" alt="">

    <img src="{usa10}" alt="">
    <img src="{usa11}" alt="">
    <img src="{usa5}" alt="">
    <img src="{usa9}" alt="">
</div>
<style>
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

    #images {
        padding-top: 5rem;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;

    }

    #images img {
        max-height: 30rem;
        margin-bottom: 1rem;
        object-fit: contain;
        max-width: 49%;
    }

    @media screen and (max-width: 500px) {
        #images {
            flex-direction: column;
            gap: 0;
        }
        #images img {
            max-height: none;
            max-width: 100%;
        }
    }
</style>