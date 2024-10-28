<script>
    import about from '$lib/images/card/about.png'
    import theme from '$lib/images/card/theme.svg'
</script>

<section class="card">
    <p class="quote">Love brings us together,
        <br>and we would be honoured if you could join us to
        <br>celebrate the wedding of
    </p>
    <img src="{about}" alt="about" class="about">
    <div class="vertical-break"></div>
    <p>Enchanted to meet you</p>
    <div class="flex-center">
        <span class="date-text">SATURDAY</span>
        <span class="noto day">7</span>
        <span class="date-text">DECEMBER</span>
    </div>
    <span class="noto year">2024</span>
    <p class="place">TARA Kaffee & Patisserie,
        <br>Tak At 4.00 PM
    </p>
    <div class="hearts flex-center">
        <span>♡</span>
        <span>♡</span>
        <span>♡</span>
    </div>
    <span class="dress-code">DRESS CODE</span>
    <img src="{theme}" alt="theme" class="theme">
</section>

<style>

    .theme {
        margin-top: 12px;
    }
    
    .card {
        display: grid;
        justify-items: center;
        color: #7B5E49;
        padding-bottom: 50px;
        background-image: url('$lib/images/card/bg.png');
        background-size: contain;
        background-position: bottom;
        background-repeat: no-repeat;
    }

    .about {
        width: 70%;
        max-width: 310px;
    }

    .vertical-break {
        width: 0.5px;
        height: 46px;
        margin: 12px 0;
        background: #CEB197;
    }

    .flex-center {
        width: 100%;
        justify-content: center;
        align-items: center;
        display: flex;
        margin: 0;
        padding: 0;
    }

    .date-text {
        font-family: "Cormorant";
        font-size: 18px;
        font-weight: 500;
        text-align: center;
        border-bottom: 0.5px solid #7B5E49;
        border-top: 0.5px solid #7B5E49;
    }

    .noto {
        font-family: "Noto Serif";
        text-align: center;
    }

    .day {
        font-size: 60px;
        font-weight: 500;
        line-height: 60px;
        margin: 0 12px;
    }

    .year {
        font-size: 20px;
        font-weight: 500;
        line-height: 20px;
    }

    p {
        font-family: "Poppins";
        font-weight: 300;
        text-align: center;
        font-size: 11px;
        margin: 0;
    }

    .quote {
        padding: 32px 0;
    }

    .place {
        margin-top: 12px;
    }

    .hearts {
        font-size: 12px;
        color: #D8A7AD;
        margin: 12px 0;
        & > span {
            margin: 0 5px;
        }
    }

    .dress-code {
        font-family: "Cormorant";
        font-size: 24px;
        font-weight: 600;
        text-align: center;
    }
</style>