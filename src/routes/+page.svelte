<script>
    import Header from "./Header.svelte";
    import Card from "./Card.svelte";
</script>

<svelte:head>
    <title>Aom & Yoke Wedding</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin=true>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300..700;1,300..700&family=Noto+Serif:ital,wght@0,100..900;1,100..900&family=Poppins:wght@300&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0 auto;
            padding: 0;
            width: 100%;
            max-width: 480px;
            height: 100vh;
            background: #F9F6F2;
        }

    </style>
</svelte:head>


<Header />
<Card />
