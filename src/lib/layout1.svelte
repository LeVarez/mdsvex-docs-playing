<script lang="ts">
    import Header from "../components/Header.svelte";
    import styles from "./styles/layout1.css"; //For some reason svelte doesn't let me overwrite the p styles if it isn't used in this file
    export let title = "No title";
</script>


<Header {title}/>
<div class="layout1">
    <slot/>
</div>

<style>
    .layout1{
        font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        padding: 35px 10% 0px 10%;
        height: 100%;
        background-color: rgb(230, 230, 230);
    }
    .ProseMirror{
        width: 400px;
    }
</style>