<script>
    import header from '$lib/images/gallery/header.webp'
    import Location from './gallery/Location.svelte'
</script>

<section id="gallery">
    <img src="{header}" alt="header" class="header">
    <div class="gallery">
        <h2>PHOTO GALLERY</h2>
        <Location caption="London, England" url="none"/>
    </div>    
</section>

<style>
    #gallery {
        width: 100%;
        font-family: "Cormorant";
    }

    .header {
        width: 100%;
    }

</style>