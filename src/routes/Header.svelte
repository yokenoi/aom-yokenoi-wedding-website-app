<script>
    import background from '$lib/images/header/home_bg.png'
    import logo from '$lib/images/header/logo.svg'
    import banner from '$lib/images/header/banner.svg'
</script>

<header>
    <img src="{background}" alt="bg_img">
    <div class="container">
        <nav>
            <img class="logo" src="{logo}" alt="logo">
        </nav>
        <img src="{banner}" alt="" class="date">
        <p>#YokeFoundHisAom</p>
    </div>
        
</header>

<style>
    .container {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        display: grid;
        justify-items: center;
        grid-template-rows: 18% 74% 8%;
        gap: 0;
    }
    
    header {
        width: 100%;
        margin-bottom: -4px;
        position: relative;
        background-image: url("$lib/images/header/home_bg.png");
        background-size: contain;
        background-repeat: no-repeat;
        & > img {
            width: 100%;
            opacity: 0;
        }
    }
    
    .date {
        width: 58%;
        margin-top: 5%;
    }

    .logo {
        width: 20%;
    }

    nav {
        width: 100%;
        max-width: 480px;
        display: flex;
        justify-content: center;
    }

    p {
        font-family: "Cormorant", serif;
        color: white;
        font-size: 18px;
        font-style: italic;
        line-height: 0;
        font-weight: 300;
    }
    
</style>