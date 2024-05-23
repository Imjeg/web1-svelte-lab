<script>
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

<div class="container">
    <header><Header /></header>
    <div class="left-side"><Sidebar {navItems} />
        <main>
            <slot />
        </main>
        <footer><Footer /></footer>
    </div>
</div>


<style>
    .container{
        display: flex;
        gap: 3em;
    }
</style>