<svelte:head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <!-- <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin> -->
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400..700&family=Wittgenstein:ital,wght@0,400..900;1,400..900&display=swap" rel="stylesheet">
</svelte:head>


<header>
    <div>
        <h1>Aom & Yoke</h1>
        <p>The wedding</p>
        <h2>Coming Soon...</h2> 
    </div>
</header>

<style>

    header {
        width: 100%;
        height: 100vh;
        display: grid;
        place-items: center; /* new */
        text-align: center;
        background-color: rgb(255, 235, 208);
    }

    div > * {
        margin: 0;
        padding: 0;
        font-family: "Dancing Script", cursive;
        font-optical-sizing: auto;
        font-style: normal;
        color: #604d15;
    }

    h2 {
        margin: 20px;
    }

    p {
        font-size: 20px;
    }
</style>