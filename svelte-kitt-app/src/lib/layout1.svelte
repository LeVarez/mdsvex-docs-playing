<script lang="ts">
import { each, end_hydrating } from "svelte/internal";


    export let title = "No title";
    export let categories = []
</script>

<div class="layout1">
    <h1>I'm using the layout1, with title: {title}</h1>
    <p>
        The {categories.length > 1? "catagories  are" : "catagory is"}:
        {#each categories as catergory}
            <li>
                {catergory}
            </li>
        {/each}
    </p>

    <slot/>
</div>

<style>
    h1{
        color: chartreuse;
    }
    .layout1{
        background-color: brown;
    }
</style>