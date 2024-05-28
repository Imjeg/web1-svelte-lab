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
        margin: 0;
        padding: 0;
        display: grid;
        grid-template: auto 1fr auto / auto 1fr;
        gap: 0px;
    }
</style>