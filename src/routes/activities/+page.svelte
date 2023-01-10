<script>
  import Footer from "../footer.svelte";
  import CardTemplate from "./card-template.svelte";

</script>

<svelte:head>
    <title>Golden Link College | Activities</title>
</svelte:head>

<main>
    <div class="container card bg bg-transparent mx-auto">
        <div id="programs" class='p-3 '>
            <h1>PROGRAMS</h1>
            <p>Every year, the Golden Link College holds the following programs and activities. The parents and the public are invited in almost all of them:</p>
            <div class="row row-cols-1 row-cols-md-3 g-4">
               <CardTemplate>
                    <img slot='img' src="/unday.jpg" alt="United Nation Day" class="card-img-top">
                    <h3 slot='title'>United Nation</h3>
                    <p slot='text'>Students wear the national dresses of different countries and have a parade through the streets, after which a UN Day Program is held in the school.</p>
               </CardTemplate>
               <CardTemplate>
                   <img slot='img' src="/buwan_ng_wika.jpg" alt="Buwan ng Wika 2015" class="card-img-top">
                   <h3 slot='title'>National Language Day (Buwan ng Wika)</h3>
                   <p slot='text'>This is a program promoting the use of Filipino. A program is also held by the students.</p>
               </CardTemplate>
               <CardTemplate>
                    <img slot='img' src="/family_day.jpg" alt="Family Day 4" class="card-img-top ">
                    <h3 slot='title'>Family Day</h3>
                    <p slot='text'>A fun day of games, activities and performances involving the entire family.</p>
                </CardTemplate>
               <CardTemplate>
                    <img slot='img' src="/declamation.jpg" alt="Declamation Day 2013" class="card-img-top">
                    <h3 slot='title'>Declamation Program</h3>
                    <p slot='text'>All students deliver their written poems or speeches.</p>
                </CardTemplate>
                <CardTemplate>
                    <img slot='img' src="/year_end.jpg" alt="Year End 2022" class="card-img-top">
                    <h3 slot='title'>Year End Program </h3>
                    <p slot='text'>Another occasion where students prepare dramas, songs, speeches, with their parents in attendance.</p>
                </CardTemplate>
                <CardTemplate>
                    <img slot='img' src="/commencement_day.jpg" alt="Commencement Day 2014" class="card-img-top">
                    <h3 slot='title'>Commencement Exercises</h3>
                    <p slot='text'>Graduation day and another occasion for dramas and speeches for the students.</p>
                </CardTemplate>
                
            </div>
        </div>
        <!-- end of program -->
        <div id="community" class='p-3'>
            <h1>Community Involvement and Services</h1>
            <div class="row row-cols-1 row-cols-2 g-4">
                <div id="carouselExampleInterval" class="carousel slide col-12 mx-auto p-3" data-bs-ride="carousel">
                    <div class="carousel-inner">
                      <div class="carousel-item active" data-bs-interval="2000">
                        <img src="/community_service.jpg" class="d-block w-100 rounded" alt="Gift Giving Nov 8,2022">
                      </div>
                      <div class="carousel-item" data-bs-interval="2000">
                        <img  src="/caroling.jpg" alt="Gift Giving Day 2014" class="d-block w-100 rounded" >
                      </div>
                      <div class="carousel-item" data-bs-interval="2000">
                        <img  src="/teaching332014.jpg" alt="Student Teacher teaching,2014" class="d-block w-100 rounded" >
                      </div>
                    </div>
                    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="prev">
                      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                      <span class="visually-hidden">Previous</span>
                    </button>
                    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="next">
                      <span class="carousel-control-next-icon" aria-hidden="true"></span>
                      <span class="visually-hidden">Next</span>
                    </button>
                  </div>
                  <div class="col-12">
                    <p>The School does not limit itself to serving its student population. It undertakes regular activities that seeks to help the community, such as:</p>
                    <p><span class='fw-bold'>Annual medical mission </span>for the community, including x-rays, dental services (including dentures), opthalmological services (with free reading glasses), immunization, deworming, and free medicine.</p>
                    <p><span class='fw-bold'>Assisting nearby public high schools</span>  in conducting teacher's training, donation of library books, holding youth camps, and conducting sessions for students.</p>
                    <p><span class='fw-bold'>Caroling to extremely poor families</span> and donating food and fund for December.</p>
                    <h4 class='mt-4'>Free Summer Classes & Youth Camp</h4>
                    <p>Every year, the College gives a one-month Summer Class for students from preschool to high school. It is completely free. Many parents send their children to these classes even though they live very far away. Some would even rent rooms nearby just to enable their children to attend these summer classes.</p>
                    <p>The focus of these classes is on language skills and personality development. It culminates in a two-day program where all the students deliver their speeches in front of the their parents, family members and guests.</p>
                    <p>The Golden Link College also conducts a 4-day youth camp to its students as well as to other interested young people.They are taught self-awareness, effective relationships and other life skills that they have invariably found to be very valuable in their lives.</p>
                    
                    <p class='mt-2'>These are in addition to the other social welfare services conducted by the Theosophical Order of Service to the community. </p>
                </div>
           </div>
        </div>
        <!-- end of community -->
    </div>
</main>
<Footer/>
<style>
    #community{
        margin-top:5rem;
    }
    main div{
        margin-bottom: 1rem;
    }
    .card-img-top {
        width: 100%;
        height: 30vh;
        object-fit: contain;
        object-fit: cover;
    }
    .carousel-item img {
        width: 100%;
        height: 25rem;
        object-fit: contain;
        object-fit: cover;
    }
</style>