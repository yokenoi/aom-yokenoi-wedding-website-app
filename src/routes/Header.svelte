<script>
    import img from '$lib/images/header/home_bg.png'
    import logo from '$lib/images/header/logo.svg'
    import banner from '$lib/images/header/banner.svg'
</script>

<header>
    <img src="{img}" alt="bg_img">
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
        width: 100%;
        height: 100%;
        max-width: 480px;
        max-height: 1038px;
        margin: 0;
        padding: 0;
        display: flex;
        align-items: center;
        justify-content: space-between;
        flex-direction: column;
    }
    
    header {
        width: 100%;
        height: 100%;
        max-height: 1038px;
        & > img {
            width: 100%;
            height: 100%;
        }
    }
    
    .date {
        position: relative;
        width: 58%;
        bottom: 20%;
    }

    nav {
        width: 100%;
        max-width: 480px;
        position: relative;
        top: 5%;
        /* background-color: red; */
        text-align: center;
    }

    p {
        font-family: "Cormorant", serif;
        color: white;
        font-size: 18px;
        font-style: italic;
        position: relative;
        bottom: 5%;
    }



</style>