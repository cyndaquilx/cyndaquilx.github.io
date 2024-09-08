<script>
    import "../app.css";
    import NavBar from "$lib/components/NavBar.svelte";
</script>

<header>
    <NavBar/>
</header>
<div class="container md:mx-auto">
    <main>
        <slot/>
    </main>
</div>

<style>
    main {
        padding-top: 25px;
    }
</style>