<script>
    import background from '$lib/images/header/bg.webp'
    import logo from '$lib/images/header/logo.svg'
    import banner from '$lib/images/header/banner.svg'

    import Menu from './Menu.svelte';

    let menuState = $state(false)
    const changeState = () => menuState = !menuState
</script>

<Menu display={menuState ? "initial" : "none"} changeState={changeState}/>

<header>
    <img src="{background}" class="background" alt="bg_img">
    <div class="container">
        <div class="header">
            <button aria-label="menu" onclick={changeState}>
                <svg width="24" height="18" viewBox="0 0 24 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect width="24" height="3" rx="1" fill="white"/>
                    <rect y="15" width="18" height="3" rx="1" fill="white"/>
                </svg>
            </button>
            <img class="logo" src="{logo}" alt="logo">
        </div>
        <img src="{banner}" alt="" class="date">
        <p>#YokeFoundHisAom</p>
    </div>
</header>




<style>

    button {
        padding: 0;
        margin: 0;
        background: none;
        border: none;
    }

    button:hover {
        cursor: pointer;
    }

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
        background-image: url("$lib/images/header/bg.webp");
        background-size: contain;
        background-repeat: no-repeat;
        & > .background {
            width: 100%;
            opacity: 0;
        }
    }
    
    .date {
        width: 58%;
        margin-top: 8%;
    }

    .logo {
        width: 29.41%;
    }

    .header {
        width: 100%;
        max-width: 480px;
        display: grid;
        justify-items: center;
        align-content: center;
        grid-template-columns: 16% 68% 16%;
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