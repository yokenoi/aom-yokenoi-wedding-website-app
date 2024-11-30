<script>
    import Location from './gallery/Location.svelte'
    import londonCard from '$lib/images/gallery/london/AY-287.webp'
    import chiangmaiCard from '$lib/images/gallery/chiangmai/AY_PRE-WEDDING_CNX_001.webp'
</script>

<section id="gallery">
    <div class="gallery">
        <h2>PHOTO GALLERY</h2>
        <div>
            <Location caption="London, England" img={londonCard} url="gallery/london"/>
            <Location caption="Chiang Mai, Thailand" img={chiangmaiCard} url="gallery/chiangmai"/>
        </div>
    </div>    
</section>

<style>
    #gallery {
        width: 100%;
        font-family: "Cormorant";
        background-image: url('$lib/images/gallery/header.webp');
        background-size: contain;
        background-repeat: no-repeat;
        background-color: #F9F6F2;
    }

    h2 {
        color: white;
        text-decoration: none;
        font-family: 600;
        font-size: 24px;
        line-height: 28px;
        margin: 0 0 12px 0;
    }

    .gallery {
        display: grid;
        justify-items: center;
        padding-top: 38%;

        & > div {
            width: 100%;
            display: flex;
            justify-content: center;
        }
    }

</style>