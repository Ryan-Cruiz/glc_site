<script>
    import Footer from '../footer.svelte';
</script>
<svelte:head>
    <title>Golden Link College | Courses</title>
</svelte:head>

<main class="pb-4">
    <div class="container row mx-auto ">
       <!-- pre -->
       <div class="col-md-5 mx-auto">
           <div class="mt-4 ms-4 card h-100 p-3 pt-0 ">
               <h4 class="card-title"><strong>Preschool</strong></h4>
               <div class="flex">
                   <span class="badge rounded-pill text-bg-none text-black">Main Campus</span>
                   <span class="badge rounded-pill text-bg-none text-black">Bohol Campus</span>
                   <span class="badge rounded-pill text-bg-none text-black">Quezon Campus</span>
               </div>
               <div class="card-body">
                   <ul>
                       <li>Nursery</li>
                       <li>Kinder 1</li>
                       <li>Kinder 2</li>
                   </ul>
               </div>
           </div>
       </div>
        <!-- pre end -->
        <!-- elem -->
        <div class="col-md-5 mx-auto">
            <div id='elem' class="mt-4 ms-4 card h-100 p-3 pt-0 ">
                <h4 class="card-title"><strong>Elementary</strong></h4>
                <div class="flex">
                    <span class="badge rounded-pill text-bg-none text-black">Main Campus</span>
                    <span class="badge rounded-pill text-bg-none text-black">Bohol Campus (up to Grade 5)</span>
                </div>
                <div class="card-body">
                    <ul>
                        <li>Grade 1</li>
                        <li>Grade 2</li>
                        <li>Grade 3</li>
                        <li>Grade 4</li>
                        <li>Grade 5</li>
                        <li>Grade 6</li>
                    </ul>
                </div>
            </div>
        </div>
        <!-- elem end -->
        <!-- jhs -->
        <div class="col-md-5 mx-auto">
            <div id="jhs" class="mt-4 card ms-4 p-3 pt-0 h-100 ">
                <h4 class="card-title"><strong>Junior High School</strong></h4>
                <div class="flex">
                    <span class="badge rounded-pill text-bg-none text-black">Main Campus</span>
                </div>
                <div class="card-body">
                    <ul>
                        <li>Grade 7</li>
                        <li>Grade 8</li>
                        <li>Grade 9</li>
                        <li>Grade 10</li>
                    </ul>
                </div>
            </div>
        </div>
        <!-- jsh end -->

        <!-- shs -->
        <div class="col-md-5 mx-auto">

            <div id="shs" class="mt-4 ms-4 card p-3 pt-0 h-100 ">
                <h4 class="card-title"><strong>Senior High School</strong></h4>
                <div class="flex">
                    <span class="badge rounded-pill text-bg-none text-black">Main Campus</span>
                </div>
                <div class="card-body">
                    <div class="accordion accordion-flush" id="shsAccordion">
                        <div class="accordion-item">
                            <h2 class="accordion-header" id="flush-head-acad">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#flush-academic" aria-expanded="false" aria-controls="flush-academic">
                                    Academic Courses
                                </button>
                            </h2>
                            <div id="flush-academic" class="accordion-collapse collapse" aria-labelledby="flush-head-acad"
                                data-bs-parent="#shsAccordion">
                                <ul>
                                    <li>Accountancy, Business, and Management (ABM) Strand</li>
                                    <li>Humanities and Social Sciences (HUMSS) Strand</li>
                                    <li>
                                        Science, Technology, Engineering, and Mathematics (STEM) Strand
                                    </li>
                                    <li>General Academic (GA) Strand</li>
                                </ul>
                            </div>
                        </div>
                        <div class="accordion-item">
                            <h2 class="accordion-header" id="flush-head-tvl">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#flush-tvl" aria-expanded="false" aria-controls="flush-tvl">
                                    TechVoc Courses
                                </button>
                            </h2>
                            <div id="flush-tvl" class="accordion-collapse collapse" aria-labelledby="flush-head-tvl"
                                data-bs-parent="#shsAccordion">
                                <ul>
                                    <li>Information and Communication Technology (ICT) Strand</li>
                                    <ol type="a">
                                        <li>Computer Programming NC IV</li>
                                        <li>Computer System Services NC II</li>
                                        <li>Animation NC II</li>
                                        <li>Illustration NC II</li>
                                    </ol>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- shs end -->

        <!-- college -->
        <div id='college' class="col-12 mx-auto">

            <div class="card list-item-college mt-4 ms-4 p-3 pt-0 ">
                <h4 class="card-title"><strong>College</strong></h4>
                <div class="flex">
                    <span class="badge rounded-pill text-bg-none text-black">Main Campus</span>
                </div>
                <!-- <h5 class='ms-3'>Courses Offered</h5> -->
                <div class="card-body">
                    <div class="accordion accordion-flush" id="collegeAccordion">
                        <div class="accordion-item">
                            <h2 class="accordion-header" id="flush-head-bsse">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#flush-bsse" aria-expanded="false" aria-controls="flush-bsse">
                                    Bachelor of info Education
                                </button>
                            </h2>
                            <div id="flush-bsse" class="accordion-collapse collapse" aria-labelledby="flush-head-bsse"
                                data-bs-parent="#collegeAccordion">
                                <ul>
                                    <li>Major in English</li>
                                    <li>Major in Mathematics</li>
                                    <li>Major in Science</li>
                                </ul>
                            </div>
                        </div>
                        <div class="accordion-item">
                            <h2 class="accordion-header" id="flush-head-bsee">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#flush-bsee" aria-expanded="false" aria-controls="flush-bsee">
                                    Bachelor of Elementary Education
                                </button>
                            </h2>
                            <div id="flush-bsee" class="accordion-collapse collapse" aria-labelledby="flush-head-bsee"
                                data-bs-parent="#collegeAccordion">
                                <ul>
                                    <li>Major in General Education</li>
                                    <li>Major in Preschool Education</li>
                                </ul>
                            </div>
                        </div>
                        <div class="accordion-item">
                            <h2 class="accordion-header" id="flush-head-bsba">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#flush-bsba" aria-expanded="false" aria-controls="flush-bsba">
                                    Bachelor of Science in business Administration
                                </button>
                            </h2>
                            <div id="flush-bsba" class="accordion-collapse collapse" aria-labelledby="flush-head-bsba"
                                data-bs-parent="#collegeAccordion">
                                <ul>
                                    <li>Major in Marketing</li>
                                </ul>
                            </div>
                        </div>
                        <ul class="list-group college-list">
                            <li class="list-group-item">BACHELOR OF SCIENCE IN PSYCHOLOGY</li>
                            <li class="list-group-item">
                                BACHELOR OF SCIENCE IN INFORMATION TECHNOLOGY
                            </li>
                            <li class="list-group-item">
                                BACHELOR OF SCIENCE IN ACCOUNTING INFORMATION SYSTEM
                            </li>
                            <li class="list-group-item">
                                TEACHER CERTIFICATE PROGRAM (For college graduates who would like to
                                take Licensure Examination for Teachers)
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <!-- college end -->
        <!-- how to enroll -->
        <div class="col-12">
            <div class="card list-item-college mt-4 ms-4 p-3 pt-0 ">
                <h4 class='card-title'><strong>How to Enroll</strong></h4>
                <div class="flex">
                    <span class="badge rounded-pill text-bg-none text-black">Updated December 31, 2022</span>
                </div>
                <div class="card-body">
                    <ol class='enrollment-list'>
                        <li>Accomplish Entrance Assessment Request form:
                            <ol type='a'>
                                <li>For Preschool, Elementary, Junior High & Senior High: <a href='https://bit.ly/BEDEntranceRegistration2022-23' target="_blank" rel='noreferrer'>Click Here</a></li>
                                <li>For College: <a href="https://bit.ly/GLC-CollegeRegistration2022-23" target="_blank" rel='noreferrer'>Click Here</a></li>
                            </ol>
                        </li>
                        <li> Let the student take the on-line entrance assessment as per schedule given by GLC.</li>
                        <li>You will be notified of the result of the assessment. After receiving assessment result,
                            <ol type='a'>
                                <li>For Preschool, Elementary, Junior High & Senior High:
                                    <ul>
                                        <li>Fill up the Enrollment Registration Form <p class='ms-2'><a href="https://forms.gle/q7kVcfg69Nw1ZFUG7" target='_blank' rel='noreferrer'>Click Here</a> with the Registration Code.</p></li> 
                                    </ul>
                                </li>
                                <li>For College: 
                                    <ul>
                                        <li>The Interviewer will give you the results and further guides you for enrollment.</li>
                                    </ul>
                                </li>
                            </ol>
                        </li>
                        <li>Send scanned copies of the following to  <a href="mailto:">goldenlink2002@gmail.com</a>:
                            <ol type='a'>
                                <li>Progress card and School Clearance (if studied before)</li>
                                <li>Birth Certificate issued by PSA/NSO</li>
                                <li>ID photo 1/1 (white background)</li>
                            </ol>
                        </li>
                        <li>After GLC has received the above requirements, you will receive a breakdown of the fees that need to be paid.</li>
                        <li>Pay school fees to any of the several ways to pay (click here for instructions: <a href='http://theosophy.ph/glchowtopay.pdf'>How To Pay</a>)
                            <ol type='a'>
                                <li>Send scanned copy of your payment for GLC record</li>
                            </ol>
                        </li>
                        <li>Three (3) days after payment, secure enrolment confirmation from GLC</li>
                        <li>Secure appointment to come to GLC in August, 2021, for the following purposes:
                            <ol type='a'>
                                <li>Signing of school ID</li>
                                <li>Signing of enrolment agreement</li>
                                <li>Purchase of textbook (from Gr. 1 to 12)</li>
                                <li>Receive set of school supplies (for preschool)</li>
                                <li>Receive first set of worksheets (for preschool)</li>
                            </ol>
                        </li>
                    </ol>
                    <p>Enrollment Complete!</p>
                </div>
            </div>
        </div>
        <!-- enroll end -->
    </div>
</main>
<Footer/>
<style>
    .card{
        background: none;
        /* border:none; */
    }
    .accordion-item{
        background:none;
        border:1px solid rgba(0, 0, 0, 0.164);
        margin:2px;
        border-radius: 5px;
    }
    .accordion-button{
        background: none;
    }
    .college-list li{
        background: none;
    }
    .badge{
        border:1px solid rgba(0, 0, 0, 0.527)
    }
    .card-title{
        padding-top:10px;
    }
    .col-md-5,#college{
        margin:5px;
    }
    .enrollment-list > li {
        padding:10px;
    }
    
</style>