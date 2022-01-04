<script lang="ts">
    export let title = "No Title";
    export let imgPath = "src/lib/img/molinos-eolicos-mar.jpg";
    export let imgAlt = "No description provided";
</script>

<div class="header">
    <h1 class="title">{title}</h1>
    <img class="img"src={imgPath} alt={imgAlt}>
</div>

<style>
    .header{
        width: 100%;
        text-align: center;
        color: rgb(29, 29, 29);
        height: 400px;
    }
    .img{
        width: inherit;
        height: 400px;
    }
    .title{
        font-size: 100px;
        color: white;
        text-shadow: 1px 1px 1px black;
        position: absolute;
        top: 15%;
        left:  50%;
        -webkit-transform: translate(-50%, -50%); /* iOS */
        transform: translate(-50%, -50%);
    }
</style>
