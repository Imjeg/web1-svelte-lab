<script>
    import Sidebar from "../../components/Sidebar.svelte";
    let navItems = [
    { text: "Home", href: "/" },
    { text: "Browse", href: "/cards/browse" },
    { text: "Manage", href: "/cards/manage" },
  ];
</script>

<Sidebar {navItems} />

<section>
    <slot />
</section>

<style>
</style>
