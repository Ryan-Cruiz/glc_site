<svelte:head>
    <title>Golden Link College | Contact Us</title>
</svelte:head>
<main>
    <div class="parallax"></div>
    <div style="height:1000px;background-color:red;font-size:36px">
        Scroll Up and Down this page to see the parallax scrolling effect.
        This div is just here to enable scrolling.
        Tip: Try to remove the background-attachment property to remove the scrolling effect.
        </div>
</main>

<style>
.parallax {
    /* The image used */
    background-image: url("/main_campus.png");

    /* Full height */
    min-height: 800px;

    /* Create the parallax scrolling effect */
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
</style>