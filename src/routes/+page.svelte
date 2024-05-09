<script>
    import Card from '../components/Card.svelte' ;
    import Header from '../components/Header.svelte';
</script>


    <Header />

<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<section>
    <Card />
    <Card />
    
</section>


<style>
    section{
        display: flex;
        gap: 3em;
    }
</style>