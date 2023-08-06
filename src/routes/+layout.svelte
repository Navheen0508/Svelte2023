<svelte:head>
    <link rel="stylesheet" href="main.css">
</svelte:head>

<p>I am the layout file</p>
<script>
    import Header  from "$lib/Header.svelte";
</script>

<Header/>

<slot/>

<footer>

    <p> Made by Navheen</p>

</footer>