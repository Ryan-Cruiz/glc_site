<script>
    import { page } from '$app/stores';
    let y,sticky,path;
    $: if (y > 0){
        sticky = 'sticky';
    }else{
        sticky = '';
    }
    $: path = $page.url.pathname;
</script>
<header class="container-fluid navbar navbar-expand-md bg-light {sticky} mb-3 py-0" >
    <div class="container-fluid">
        <a class="navbar-brand" href="/">
            <img src="/favicon.png" width="60" height="60" class="d-inline-block align-top" alt="">
            <div class="d-inline-block mt-3">
                <h6>Golden Link College</h6>
            </div>
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="mx-auto collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0" id='nav-ul'>
            <li class="nav-item">
                <a class:is-active={$page.url.pathname === "/"} class="nav-link" aria-current="page" href="/">Home</a>
            </li>
            <li class="nav-item">
                <a class:is-active={$page.url.pathname === "/courses"} class="nav-link" href="/courses">Courses</a>
            </li>
            <li class="nav-item">
                <a class:is-active={$page.url.pathname === "/news"} href="/news" class="nav-link">News</a>
            </li>
            <li class="nav-item">
                <a class:is-active={$page.url.pathname === "/activities"} class="nav-link" href="/activities">Activities</a>
            </li>
            <li class="nav-item">
                <a class:is-active={$page.url.pathname === "/about"} href="/about" class="nav-link">About</a>
            </li>
        </div>
    </div>
</header>
<svelte:window bind:scrollY={y}></svelte:window>
<style>
    .is-active {
        color: #1B74E4;
        border-bottom: 2px solid #1B74E4;
    }
    .nav-link:hover {
        background-color: #E3E5E8;
        color:black;
    }
    @media (max-width: 800px) {
		#nav-ul > li > a {
			text-align: center;
		}
	}
    .sticky {
        position: fixed;
        top: 0;
        width: 100%;
    }
    .sticky + .content {
        padding-top: 102px;
    }
    header{
        clear: both;
        z-index: 9999;/* set this to something high*/
    }
    /* .container-fluid{
        background: rgba(51, 170, 51, .1);
    } */
</style>

<div class='content'>
    <slot/>
</div>