<script>
    import Card from '../components/Card.svelte' ;
    import Header from '../components/Header.svelte';
    import Footer from '../components/Footer.svelte';
    import Sidebar from '../components/Sidebar.svelte';

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
    section{
        display: flex;
        gap: 3em;
    }
</style>