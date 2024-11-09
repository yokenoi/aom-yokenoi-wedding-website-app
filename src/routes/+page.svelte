<script>
    import Menu from "./Menu.svelte";
    import Header from "./Header.svelte";
    import About from "./About.svelte";
    import Gallery from "./Gallery.svelte";
    import metaImage from '$lib/images/meta_image.webp'

    let menuState = $state(false);
    
    
    
</script>

<svelte:head>
    <title>Aom & Yoke Wedding</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+SC:wght@300;500;600&family=Cormorant:ital,wght@0,300..700;1,300..700&family=Noto+Serif:ital,wght@0,100..900;1,100..900&family=Poppins:wght@300&display=swap" rel="stylesheet">
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