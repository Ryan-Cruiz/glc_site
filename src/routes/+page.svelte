<script>
  import Footer from "./footer.svelte";

</script>
<svelte:head>
    <title>Golden Link College</title>
</svelte:head>
<main>
    <div class='container school-name full-bleed row mx-auto '>
        <div class='col-md-5 d-flex align-self-center justify-content-center'>
            <div class='school-name-container'>
                <h1 class="ps-3 mx-auto">Golden Link College</h1>
                <h5>A vision of transformative education</h5>
            </div>
        </div>
        <div class="col-md-6 text-center mx-auto d-flex align-items-center justify-content-center">
            <img src="/glcwebpic.jpg" alt="main campus school ground" class='mh-100 '>
        </div>
    </div>
    <div class='mt-5 container-sm'>
        <div class="p-5 m-5 mx-auto mission-vision">
            <h2>The Golden Link College</h2>
            <h5 class='mt-3 ps-4'>Adopts an educational approach that:</h5>
            <ul class='ps-4'>
                <li>Gives importance to the development of life skills and character building, such as self-awareness, integration of values, effective relationships, conflict resolution, public speaking, etc., side by side with academic competencies.</li>
                <li>Motivates students to study by awakening their interest in the subject matter instead of using rewards and punishments or threats.</li>
                <li>Creates an atmosphere of care, fun and challenge that enables students to dare to try new things without the fear of being humiliated or punished.</li>
                <li>Does not use rankings, honors or medals to compare a student with another.</li>
                <li>Involves the parents and family in the education of the children, by holding parenting seminars and family day programs.</li>
                <li>Enables students to be aware of the larger picture such as the environment, meaning of life, comparative religion, world peace and similar themes. </li>
            </ul>
        </div>
    </div>
    <div class='mt-5 container-sm'>
        <div class="p-5 m-5 mx-auto mission-vision">
            <h2>Mission and Vision</h2>
            <ul class='ps-3'>
                <li>To educate and bring up children and young adults to become competent, well balanced, emotionally mature, socially responsible, morally upright and spiritually sensitive individuals.</li>
                <li>To develop and promote an enlightened educational system that teaches the art and science of wise living in addition to achieving academic excellence.</li>
                <li>A system that can be shared with other institutions for the benefit of individuals and society.</li>
                <li>To be a center of peace and harmony where people of different cultures will leave and learn together to help promote world peace and brotherhood without distinction of religion, race, sex or nationality, in the light of the ageless wisdom of life.</li>
                <li>To help provide quality and right education to the less privileged children.</li>
            </ul>
        </div>
    </div>
</main>
<Footer/>
<style>
    *{
        font-family: Arial, Helvetica, sans-serif;
        padding: 0px;
        margin:0px;
    }
    .mission-vision ul li{
        margin:10px;
    }
    .school-name{

        text-align: center;
        height: 60ch;
        margin-bottom: 5rem;
    }
    /* .full-bleed{
        box-shadow: 0 0 0 100vmax #40739e;
        clip-path: inset(0 -100vmax);
    } */
    .school-name-container h1{
        font-size: 50px;
    }

</style>