<script>
    import Card from '../components/Card.svelte' ;
    

    let navItems =[
    {text: "Home", href: "/"},
    {text: "About", href: "/about"},
    {text: "My Cards", href: "/cards"},
    {text: "Contact", href: "/contact"},
   ];
</script>


    <Header />
    <Sidebar {navItems} />

<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<section>
    <Card />
    <Card />
    
</section>

<Footer />

<style>
    
</style>