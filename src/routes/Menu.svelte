<script>
    import logo from '$lib/images/header/logo.svg'
    import bgTop from '$lib/images/menu/bq_top.webp'
    import bgBottom from '$lib/images/menu/bg_bottom.webp'

    let { display, changeState } = $props()
    const menus = [
        ["#about", "About"],
        ["#gallery", "Photo Gallery"],
        
    ]
</script>

<div class="container" style="display: {display};">
    <img class="bg-top" src="{bgTop}" alt="logo">
    <div>
        <img class="logo" src="{logo}" alt="logo">
        <div class="menu">
            {#each menus as menu}
                <a href={menu[0]} onclick={changeState}>{menu[1]}</a>
            {/each}
        </div>
        <span>♡</span>
    </div>
    <img class="bg-bottom" src="{bgBottom}" alt="bottom">
</div>


<style>
    .container {
        background-color: #6E7A58;
        position: fixed;
        width: 100%;
        max-width: 480px;
        height: 100vh;
        z-index: 1;

        & > div {
            display: grid;
            justify-items: center;
            align-items: center;
            grid-template-rows: 20vh 60vh 20vh;
        }
    }

    .menu {
        font-family: "Poppins";
        font-weight: 300;
        font-size: 20px;
        text-align: center;
        list-style-type: none;
        display: flex;
        flex-direction: column;
        gap: 50px;
    }

    a {
        color: white;
        text-decoration: none;
    }

    .logo {
        width: 20%;
    }

    .bg-top {
        max-width: 37.2%;
        position: absolute;
    }

    .bg-bottom {
        max-width: 40%;
        position: absolute;
        bottom: 0;
        right: 0;
    }

    span {
        font-size: 16px;
        color: white;
    }


</style>