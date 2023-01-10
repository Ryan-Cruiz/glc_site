<script>
    import CardTemplate from "./activities/card-template.svelte";
    import Footer from "./footer.svelte";
    let img_desc = ['comlab 2','BSBA and BSAIS taking exam','Psych Pinning 2022','Education Major On Laugh Out Loud']
    let images = ['comlab_2.jpg','bsba.jpeg','psych_pinning.jpg','educ.jpeg'];
    let courses = ['Information Technology','Business Administration and Accounting Information System','Psychology','Primary and Secondary Education'];
    let ms = 3000
    let counter = 0
    const incr = () => (counter += 1)
    $: if(counter == courses.length){
        counter = 0;
    }
    let clear
    $: {
        clearInterval(clear)
        clear = setInterval(incr, ms)
    }
</script>
<svelte:head>
    <title>Golden Link College</title>
</svelte:head>
<main>
    <div class='school-name mx-auto'>
        <div class='school-name-container m-4 mx-auto '>
            <h1 class="ps-3 mx-auto fw-bold">Golden Link College</h1>
            <h5 class='fs-4 mt-2'>A vision of transformative education</h5>
        </div>
    </div>
    <div class="bg-img container-fluid">
        <img src="/glc_orientation.jpg" alt="glc orientation 2022" class='w-100'>
    </div>
    <div class="container-md mx-auto mission-vision m-5">
        <h2 class=' fw-bold text-center my-3'>Mission and Vision</h2>
        <ul class='ps-3'>
            <li>To educate and bring up children and young adults to become competent, well balanced, emotionally mature, socially responsible, morally upright and spiritually sensitive individuals.</li>
            <li>To develop and promote an enlightened educational system that teaches the art and science of wise living in addition to achieving academic excellence.</li>
            <li>A system that can be shared with other institutions for the benefit of individuals and society.</li>
            <li>To be a center of peace and harmony where people of different cultures will leave and learn together to help promote world peace and brotherhood without distinction of religion, race, sex or nationality, in the light of the ageless wisdom of life.</li>
            <li>To help provide quality and right education to the less privileged children.</li>
        </ul>
    </div>
    <div class="container-md mx-auto m-3">
        <h2 class='fw-bold my-3 text-center'>Educational Approach</h2>
        <div class="approach-section">
            <ul class='list-group list-group-horizontal'>
                <li class='list-group-item ranking-icon'>
                    <svg id='rank' xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512"><!--! Font Awesome Pro 6.2.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M353.8 54.1L330.2 6.3c-3.9-8.3-16.1-8.6-20.4 0L286.2 54.1l-52.3 7.5c-9.3 1.4-13.3 12.9-6.4 19.8l38 37-9 52.1c-1.4 9.3 8.2 16.5 16.8 12.2l46.9-24.8 46.6 24.4c8.6 4.3 18.3-2.9 16.8-12.2l-9-52.1 38-36.6c6.8-6.8 2.9-18.3-6.4-19.8l-52.3-7.5zM256 256c-17.7 0-32 14.3-32 32V480c0 17.7 14.3 32 32 32H384c17.7 0 32-14.3 32-32V288c0-17.7-14.3-32-32-32H256zM32 320c-17.7 0-32 14.3-32 32V480c0 17.7 14.3 32 32 32H160c17.7 0 32-14.3 32-32V352c0-17.7-14.3-32-32-32H32zm416 96v64c0 17.7 14.3 32 32 32H608c17.7 0 32-14.3 32-32V416c0-17.7-14.3-32-32-32H480c-17.7 0-32 14.3-32 32z"/></svg>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><!--! Font Awesome Pro 6.2.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M367.2 412.5L99.5 144.8C77.1 176.1 64 214.5 64 256c0 106 86 192 192 192c41.5 0 79.9-13.1 111.2-35.5zm45.3-45.3C434.9 335.9 448 297.5 448 256c0-106-86-192-192-192c-41.5 0-79.9 13.1-111.2 35.5L412.5 367.2zM512 256c0 141.4-114.6 256-256 256S0 397.4 0 256S114.6 0 256 0S512 114.6 512 256z"/></svg>
                </li>
                <li class='list-group-item'>
                    <p>Does not use rankings, honors or medals to compare a student with another.</p>
                </li>
            </ul>

            <ul class='list-group list-group-horizontal'>
                <li class='list-group-item ranking-icon'>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512"><!--! Font Awesome Pro 6.2.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M208 352c114.9 0 208-78.8 208-176S322.9 0 208 0S0 78.8 0 176c0 38.6 14.7 74.3 39.6 103.4c-3.5 9.4-8.7 17.7-14.2 24.7c-4.8 6.2-9.7 11-13.3 14.3c-1.8 1.6-3.3 2.9-4.3 3.7c-.5 .4-.9 .7-1.1 .8l-.2 .2 0 0 0 0C1 327.2-1.4 334.4 .8 340.9S9.1 352 16 352c21.8 0 43.8-5.6 62.1-12.5c9.2-3.5 17.8-7.4 25.3-11.4C134.1 343.3 169.8 352 208 352zM448 176c0 112.3-99.1 196.9-216.5 207C255.8 457.4 336.4 512 432 512c38.2 0 73.9-8.7 104.7-23.9c7.5 4 16 7.9 25.2 11.4c18.3 6.9 40.3 12.5 62.1 12.5c6.9 0 13.1-4.5 15.2-11.1c2.1-6.6-.2-13.8-5.8-17.9l0 0 0 0-.2-.2c-.2-.2-.6-.4-1.1-.8c-1-.8-2.5-2-4.3-3.7c-3.6-3.3-8.5-8.1-13.3-14.3c-5.5-7-10.7-15.4-14.2-24.7c24.9-29 39.6-64.7 39.6-103.4c0-92.8-84.9-168.9-192.6-175.5c.4 5.1 .6 10.3 .6 15.5z"/></svg>
                </li>
                <li class='list-group-item'>
                    <p>Gives importance to the development of life skills and character building, such as self-awareness, integration of values, effective relationships, conflict resolution, public speaking, etc., side by side with academic competencies.</p>
                </li>
            </ul>

            <ul class='list-group list-group-horizontal'>
                <li class='list-group-item ranking-icon'>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><!--! Font Awesome Pro 6.2.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M416 208c0 45.9-14.9 88.3-40 122.7L502.6 457.4c12.5 12.5 12.5 32.8 0 45.3s-32.8 12.5-45.3 0L330.7 376c-34.4 25.2-76.8 40-122.7 40C93.1 416 0 322.9 0 208S93.1 0 208 0S416 93.1 416 208zM208 352c79.5 0 144-64.5 144-144s-64.5-144-144-144S64 128.5 64 208s64.5 144 144 144z"/></svg>
                </li>
                <li class='list-group-item'>
                    <p>Motivates students to study by awakening their interest in the subject matter instead of using rewards and punishments or threats.</p>
                </li>
            </ul>
        </div>
    </div>
    <div class="container-md mx-auto m-3">
        <h2 class=" fw-bold my-3 text-center">Courses Offered</h2>
        <div class='row row-cols-1 row-cols-md-2 g-4 justify-content-center'>
            <CardTemplate>
                <img slot='img' src="/{images[counter]}" alt="{img_desc[counter]}">
                <h4 slot='title' class='text-center'>
                {#if courses[counter] == 'Primary and Secondary Education'}
                    Bachelor of {courses[counter]}
                {:else}
                   Bachelor of Science in {courses[counter]}
                {/if}
                </h4>
                <p slot='text'></p>
            </CardTemplate>
        </div>
        <a href='/courses' class="text-center mx-auto d-block btn btn-primary p-2 w-50 mx-auto m-3">See More</a>
    </div>
</main>
<Footer/>
<style>
    *{
        font-family: Arial, Helvetica, sans-serif;
        padding: 0px;
        margin:0px;
    }
    li{
        font-size:20px;
    }
    .mission-vision ul li{
        margin:12px;
    }
    .school-name{
        height:60ch;
        display:flex;
        justify-items: center;
        align-items: center;
        text-align: center;
    }
    .school-name-container h1{
        font-size: 50px;
    }
    .bg-img{
        height: 60ch;
    }
    .bg-img img{
        /* background-image: url('/glc_orientation.jpg'); */
        height: 100%;
    
        /* Center and scale the image nicely */
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        object-fit: cover;
    }
    .ranking-icon svg{
        height: 6rem;
        width: 6rem;
    }
        #rank{
         position:absolute;   
        }
    .approach-section ul li {
        background: none;
        border:none;
        margin:20px;
        display:flex;
        align-items: center;
        justify-items: center;
    }
</style>
