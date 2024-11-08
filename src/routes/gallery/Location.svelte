<script>
    let { caption, img="", url="" } = $props();

</script>


<div class="card">
    <div class="image" style:background-image='url({img})'></div>
    <div class="vertical-break"></div>
    <span>{caption}</span>
     <a href={url}>View</a>
</div>

<style>

    .vertical-break {
        width: 0.5px;
        height: 14px;
        background-color: #CEB197;
        margin: 8px 0 4px 0;
    }

    .card {
        display: grid;
        justify-items: center;
        text-align: center;
        width: 32%;
        margin: 0 5%;
    }

    .image {
        width: 100%;
        padding-top: 150%;
        background-size: cover;
        background-position: center;
    }
    
    a {
        font-family: "Poppins";
        font-weight: 300;
        line-height: 12px;
        font-size: 8px;
        color: #7B5E49;
        border: 0.5px solid #7B5E49;
        border-radius: 12px;
        text-decoration: none;
        padding: 0 8px;
        margin-bottom: 4px;
    }

    /* a:active {
        color: white;
        background-color: #7B5E49;
    } */

    span {
        font-style: italic;
        color: #6E7A58;
        font-weight: 500;
        margin-bottom: 6px;
    }
</style>