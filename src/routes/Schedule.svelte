<section id="schedule">
    <h2>OUR SPECIAL DAY'S<br>SCHEDULE</h2>
    {#each items as item}
    <div>
        <img src={item.img} alt={item.alt}>
        <span class="time">{item.time}</span>
        <p class="cation">{item.caption}</p>
    </div>
    {/each}
</section>

<style>

    #schedule {
        text-align: center;
        padding: 54px 0;
    }

    h2 {
        font-family: "Cormorant SC";
        line-height: 1;
        font-weight: 600;
        font-size: "24px";
        color: #7B5E49;
        margin-bottom: 40px;
        margin-top: 0;
        padding: 0;
    }

    div {
        display: grid;
        justify-items: center;
        margin-top: 20px;
    }

    span {
        font-family: "Noto Serif";
        font-weight: 500;
        size: 20px;
        color: #7B5E49;
    }

    p {
        line-height: 1;
        font-family: "Poppins";
        font-size: 11px;
        color: #6E7A58;
        padding: 0;
        margin: 0;
    }


</style>

<script>
    import camera from '$lib/images/schedule/camera.svg'
    import rings from '$lib/images/schedule/rings.svg'
    import party from '$lib/images/schedule/party.svg'

    const items = [
        {
            "img": camera,
            "alt": "camera",
            "time": "16:00",
            "caption": "Capture the moments"
        },
        {
            "img": rings,
            "alt": "rings",
            "time": "18:00",
            "caption": "Wedding ceremory"
        },
        {
            "img": party,
            "alt": "party",
            "time": "16:00",
            "caption": "Let's party!"
        }
    ]
</script>