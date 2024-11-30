<script>
    import Header from "./Header.svelte";
    import About from "./About.svelte";
    import Gallery from "./Gallery.svelte";
    import Schedule from "./Schedule.svelte";
    import Location from "./Location.svelte";
    import Countdown from "./Countdown.svelte";
    import Info from "./Info.svelte";
    import metaImage from '$lib/images/meta_image.webp'
</script>

<svelte:head>
    <title>Aom & Yoke Wedding</title>
    <meta property="og:image" content={metaImage}>
    <meta property="og:title" content="Aom & Yoke Wedding">
    <meta property="og:description" content="Love brings us together, and we would be honoured if you could join us to celebrate our wedding!">
    <style>
        body {
            margin: 0 auto;
            padding: 0 0 0 0;
            width: 100%;
            max-width: 480px;
            height: 100vh;
            background-color: #F9F6F2;
        }
    </style>
</svelte:head>


<Header />
<About />
<Gallery />
<Schedule />
<Location />
<Info />
<Countdown />