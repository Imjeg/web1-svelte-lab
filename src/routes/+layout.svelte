<script>
    import Header from "../components/Header.svelte";
    import Footer from "../components/Footer.svelte";
    import Sidebar from "../components/Sidebar.svelte";
    let navItems = [
      { text: "Home", href: "/" },
      { text: "About", href: "/about" },
      { text: "My Cards", href: "/cards" },
      { text: "Contact", href: "/contact" },
    ];
  </script>

  <div class="container">
    <Header {navItems} />
    <Sidebar {navItems} />
    <main>
      <slot />
    </main>
    <Footer />
  </div>

  <style>
    .container {
      display: grid;
      grid-template: auto 1fr auto / auto 1fr;
    }
  </style>