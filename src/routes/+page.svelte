<script>
    import Card from '../components/Card.svelte' ;
    export let data;
    const people = data.people;
    console.log(data.people);
    
    let navItems =[
    {text: "Home", href: "/"},
    {text: "About", href: "/about"},
    {text: "My Cards", href: "/cards"},
    {text: "Contact", href: "/contact"},
   ];
</script>

<main>
{#each people as person}
<Card {person} />
{/each}

</main>
    <Header />
    <Sidebar {navItems} />

<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<section>
    <Card />
    <Card />
    
</section>
<Footer></Footer>

<style>
    
</style>