<script>
    const imageModules = import.meta.glob("$lib/images/gallery/chiangmai/*.webp");
    // const imageUrls = []
    // for (const modulePath in imageModules) {
    //     imageModules[modulePath]().then((imageUrl) => {
    //         console.log(modulePath, imageUrl);
    //         imageUrls.push(imageUrl)
    //     });
    // }
</script>

<div class="container">
    {#each Object.values(imageModules) as importImage}
        {#await importImage() then { default: imgUrl }}
            <img src="{imgUrl}" alt="{imgUrl}">
        {/await}
    {/each}
</div>


<style>
    .container {
        width: 95%;
        max-width: 480px;
        margin: 10px auto;
        row-gap: 10px;
        display: grid;

        justify-content: center;
    }

    img {
        width: 100%;
    }
</style>