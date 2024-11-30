<script>
    const data = {
        "Accommodation": "If you asked as to book for you, the chosen hotel will be Suan Sin Lanna. Other recommended hotels are Silayok, White House, and Suan Sin Garden",
        "Transportation": "The wedding ceremony is helded 8km away from Suan Sin Lanna. Please check with bridemates or groommates.",
        "Parking": "Parking on street side is allowed. The parking lot will be reserved for family and crew members."
    }
</script>


<section id="info">
    {#each Object.entries(data) as [heading, info]}
        <div>
            <h3>{heading}</h3>
            <p>{info}</p>
        </div>
    {/each}
</section>

<style>
    #info {
        display: grid;
        justify-items: center;
        color: #7B5E49;
        row-gap: 20px;
        padding: 20px 0;
    }

    div {
        width: 80%;
        text-align: center;
        justify-items: center;
    }

    div > * {
        margin: 0;
        padding: 0;
    }

    p {
        font-family: "Poppins";
        font-weight: 300;
        font-size: 11px;
    }

    h3 {
        font-family: "Cormorant";
        font-weight: 500;
        font-size: 18px;
        line-height: 1.15;
        border: 0.5px solid #7B5E49;
        width: fit-content;
        padding: 2px 10px;
        margin-bottom: 8px;
        border-radius: 18px;
    }

</style>
