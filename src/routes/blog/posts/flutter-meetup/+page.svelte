<script>
    import flutter1 from '$lib/images/flutter1.jpg';
    import flutter2 from '$lib/images/flutter2.jpg';
    import flutter3 from '$lib/images/flutter3.jpg';
    import flutter4 from '$lib/images/flutter4.jpg';
</script>

<h1>Flutter Belgium Meetup</h1>
<h2>Introduction</h2>
<p>The recent Flutter Belgium Meetup was a dynamic event that brought together Flutter enthusiasts, developers, and experts to discuss the latest trends and technologies in the Flutter ecosystem. The event featured insightful talks from industry professionals, providing attendees with practical knowledge and inspiration for their own Flutter projects. Two standout presentations were delivered by Thijs, a Flutter developer from Cyber Tre Labs, and Enzo Conty, a senior freelance Flutter developer from Bordeaux, France.</p>
<h2>OCR and Object Detection in Flutter by Thijs</h2>
<p>Thijs, a Flutter developer at Cyber Tre Labs, shared his experience of creating his first application using object detection and OCR (Optical Character Recognition) in Flutter. The project was developed for Lum trailers, a company that manufactures trailers for transporting dry goods. Thijs's application aimed to replace an existing costly and error-prone hardware system with a more efficient and cost-effective mobile solution using Flutter.</p>
<h2>The Project</h2>
<p>The project focused on developing a smartphone application to enhance the accuracy and efficiency of unloading trailers at customer sites. Thijs detailed the process of implementing object detection to ensure that the trailer's hose was correctly connected to the silo pipe and using OCR to read the silo ID. This eliminated the need for expensive NFC tag readers and minimized human error. The solution utilized YOLO (You Only Look Once) V8 for object detection, demonstrating how to acquire data, label it, train the model, and deploy it in a Flutter application.</p>
<h2>Implementation and Challenges</h2>
<p>Thijs explained the technical steps involved in creating the application, including data acquisition, labeling, training the model with YOLO V8, and converting the model for use in Flutter. The Flutter Vision package was highlighted for its compatibility with YOLO V8, though it currently only supports Android. Despite some challenges, such as the need for better OCR performance for large single characters, the project successfully demonstrated the potential of using Flutter for complex computer vision tasks.</p>
<h2>Conclusion</h2>
<p>The project not only showcased the capabilities of Flutter in integrating advanced technologies like object detection and OCR but also highlighted practical solutions to real-world problems faced by companies like Lum trailers. Thijs's presentation provided valuable insights and inspiration for developers looking to explore similar applications in Flutter.</p>
<h2>Accessibility in Flutter by Enzo Conty</h2>
<h2>Introduction</h2>
<p>Enzo Conty, the first international speaker at Flutter Belgium, delivered an enlightening talk on accessibility in Flutter. Enzo, a senior freelance Flutter developer from Bordeaux, emphasized the importance of making applications accessible not only for people with disabilities but for all users. He highlighted the upcoming European Accessibility Act (EAA), which will mandate accessibility features in new digital products starting in 2025 and existing ones by 2030.</p>
<h2>Understanding Accessibility</h2>
<p>Accessibility involves making content and services usable for people with disabilities and improving the overall user experience. Enzo explained the different types of disabilities: sensory (e.g., blindness, hearing impairments), cognitive (e.g., dyslexia, ADHD), and mobility (e.g., reduced mobility, temporary disabilities). He debunked common myths about accessibility, such as the belief that it is only for a few users or that it makes products more expensive and complex.</p>
<h2>Practical Solutions</h2>
<p>Enzo provided practical solutions for improving accessibility in Flutter applications. For sensory disabilities, he suggested using appropriate font sizes, ensuring a high contrast ratio, and leveraging screen readers like VoiceOver and TalkBack. For cognitive disabilities, he recommended using dyslexia-friendly fonts, creating clean and streamlined interfaces, and avoiding long loading times. For mobility impairments, Enzo advised designing for one-handed use and ensuring easy access to essential UI elements.</p>
<h2>Conclusion</h2>
<p>Enzo emphasized the importance of starting accessibility efforts early in the development process to avoid costly retrofitting later. He encouraged developers to become leaders in accessibility to gain a competitive edge as regulations tighten. Enzo's talk was a call to action for developers to create more inclusive applications, benefiting not only those with disabilities but enhancing the user experience for everyone.</p>
<div id="images">
    <img src="{flutter1}" alt="">
    <img src="{flutter2}" alt="">
    <img src="{flutter3}" alt="">
    <img src="{flutter4}" alt="">
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

    a {
        text-decoration: underline;
    }
</style>