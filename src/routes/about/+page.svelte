<script>
  import Footer from "../footer.svelte";
import Profile from "./profile.svelte";

</script>
<svelte:head>
    <title>Golden Link College | Contact Us</title>
</svelte:head>
<main>
    <div class="parallax"></div>
    <div class="container">
        <div class="container pt-5">
            <div class="card bg bg-transparent">
                <div class="card-body">
                    <p>Golden Link College is an institution established by the Theosophical Society in the Philippines and the Theosophical Order of Service Foundation Philippines. It is located in the northern part of Caloocan, Philippines. As of 2009, it offers courses from preschool, elementary, secondary up to collegiate levels. It is a non-profit, non-sectarian college set up as foundation.</p>
                </div>
            </div>
            <div class="card mt-5 bg bg-transparent">
                <h3 class="card-title p-3">2002-2003</h3>
                <div class="card-body ps-5">
                    <p>June 2002 Golden Link College open their first school at Waling-waling St., Barangay 177 with pre-school classes (nursery, kindergarten, and preparatory levels). The following year, it accepted elementary school pupils. </p>
                </div>
            </div>
            <div class="card mt-5 bg bg-transparent">
                <h3 class="card-title p-3">2005-2006</h3>
                <div class="card-body ps-5">
                    <p>In 2005, it opened its secondary school department. Following year, its started its Golden Link Institute for Teacher Training as a program for training its own teachers and college students who are taking up education courses.</p>
                </div>
            </div>
            <div class="card mt-5 bg bg-transparent">
                <h3 class="card-title p-3">2009</h3>
                <div class="card-body ps-5">
                    <p>In 2009, it was given approval by the Commission on Higher Education (CHED) to open two collegiate courses: Bachelor of Secondary Education (major in English, Mathematics or Physical Sciences) and Bachelor of Elementary Education (major in General Education or Preschool Education). It added three additional courses: Bachelor of Science in Information Technology, Bachelor of Science in Business Administration (major in Marketing Management), and Bachelor of Science in Psychology.</p>
                </div>
            </div>
            <div class="card mt-5 bg bg-transparent">
                <h3 class="card-title p-3">2013-2015</h3>
                <div class="card-body ps-5">
                    <ul>
                        <li>In 2013, it was given approval by CHED to offer Teacher Certificate Program (TCP) for college graduates of non-education courses so that they can take the government Licensure Examination for Teachers. Golden Link College frequently has visiting teachers or professors from other countries (e.g., Australia, France, Switzerland) who teach short-term courses in various fields, such as leadership, literature, leadership, art, etc. It has also received grants and support from individuals and organizations for scholarships to poor students and for campus development.</li>
                        <li>In 2013, Golden Link College opened its first branch in Cortes, Bohol Province, for preschool levels: Nursery, Kindergarten 1 and Kindergarten 2. Like its mother campus, it also offered free summer classes to the community for the development of language proficiency and personality. In 2015, it opened its elementary department.</li>
                    </ul>
                </div>
            </div>
            <div class="card mt-5 bg bg-transparent mb-5">
                <h3 class="card-title p-3">Administration, Faculty and Staff</h3>
                <div class="card-body">
                    <h4 class="p-3 ps-0">Board of Trustees</h4>
                    <div id="trustees" class='mt-1 row row-cols-1 row-cols-md-3 g-4'>
                        <Profile>
                                <span slot='name'>Dr. Roselmo Doval-Santos</span>
                                <span slot='position'>Chairman</span>
                        </Profile>
                        <Profile>
                                <span slot='name'>Vicente Hao Chin, Jr.</span>
                                <span slot='position'>President</span>
                        </Profile>
                        <Profile>
                            <span slot='name'>Dr. Estrellita Gruenberg</span>
                            <span slot='position'>Vice President</span>
                        </Profile>
                        <Profile>
                            <span slot='name'>Dr. Annie Dumlao</span>
                            <!-- <span slot='position'>President</span> -->
                        </Profile>
                        <Profile>
                            <span slot='name'>Atty. Charlton Jules Romero</span>
                            <!-- <span slot='position'>President</span> -->
                        </Profile>
                    </div>
                    <h4 class='p-3 ps-0'>Administration</h4>
                    <div id="administration" class='mt-1 row row-cols-1 row-cols-md-3 g-4'>
                        <Profile>
                            <span slot='name'>Vicente Hao Chin, Jr.</span>
                            <span slot='position'>President</span>
                        </Profile>
                        <Profile>
                            <span slot='name'>Rekha L. Nahar</span>
                            <span slot='position'>Vice President and Administrator</span>
                        </Profile>
                        <Profile>
                            <span slot='name'>Dr. Estrellita Gruenberg.</span>
                            <span slot='position'>Vice President and Dean</span>
                        </Profile>
                        <Profile>
                            <span slot='name'>Eiren Galang</span>
                            <span slot='position'>Principal, Basic Education Department</span>
                        </Profile>
                        <Profile>
                            <span slot='name'>Corazon Ponteres</span>
                            <span slot='position'>Directress, Bohol Campus</span>
                        </Profile>
                        <Profile>
                            <span slot='name'>Asuncion Bispo</span>
                            <span slot='position'>Registrar</span>
                        </Profile>
                        <Profile>
                            <span slot='name'>John Derson Herbolario</span>
                            <span slot='position'>College Student Affairs Officer</span>
                        </Profile>
                        <Profile>
                            <span slot='name'>Teresita Agbay</span>
                            <span slot='position'>Librarian</span>
                        </Profile>
                        <Profile>
                            <span slot='name'>Mary Grace Arboleda</span>
                            <span slot='position'>Senior High School and Branch Coordinator</span>
                        </Profile>
                    </div>
                </div>
            </div>
    </div>
</main>
<Footer/>
<style>

.card-body ul li {
    margin-bottom: 10px;
}
.parallax {
    
    /* The image used */
    background-image: url("/main_campus.png");
    /* blur */

    /* Full height */
    min-height: 800px;
    position:relative;
    bottom:16px;
    /* Create the parallax scrolling effect */
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
</style>