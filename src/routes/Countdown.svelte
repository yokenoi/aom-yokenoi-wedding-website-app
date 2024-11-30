<script>
    let days = 0;
    let hours = 0;
    let minutes = 0;
    let seconds = 0;

    const targetTime = new Date("2024-12-07T16:00:00+0700")

    setInterval(() => {
        let time = Math.floor((targetTime.getTime() - Date.now()) / 1000)
        seconds = Math.max(time % 60, 0)
        minutes = Math.max(Math.floor(time % (60 * 60) / 60), 0)
        hours = Math.max(Math.floor(time % (60 * 60 * 24) / (60 * 60)), 0)
        days = Math.max(Math.floor(time / (60 * 60 * 24)), 0)
    }, 1000)
</script>

<section id="countdown">
    <h2>LET THE COUNTDOWN BEGIN</h2>
    <div class="clock">
        <span class="number">{days}</span>
        <span class="number">{hours}</span>
        <span class="number">{minutes}</span>
        <span class="number">{seconds}</span>
        <p class="caption">DAYS</p>
        <p class="caption">HOURS</p>
        <p class="caption">MINUTES</p>
        <p class="caption">SECONDS</p>
    </div>
</section>

<style>
    #countdown {
        height: 162px;
        width: 100%;
        background-image: url("$lib/images/countdown/bg.webp");
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;
        flex-direction: column;
    }

    h2 {
        margin: 0;
        font-family: "Cormorant SC";
        font-size: 18px;
        font-weight: 500;
    }

    .clock {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        width: 80%;
        text-align: center;
    }

    .number {
        font-family: "Noto Serif Display";
        font-weight: 500;
        font-size: 48px;
        margin: 0;
        padding: 0;
    }

    .caption {
        font-family: "Poppins";
        font-size: 11px;
        font-weight: 300;
        margin: 0;
        padding: 0;
    }
</style>