<script>
  import Card from "../components/Card.svelte";
  import Header from "../components/Header.svelte";
  import Sidebar from "../components/Sidebar.svelte";
  import Footer from "../components/Footer.svelte";

  export let data;
  const people = data.people;
  console.log(data.people);

  let navItems = [
    { text: "Home", href: "/" },
    { text: "About", href: "/about" },
    { text: "My Cards", href: "/cards" },
    { text: "Contact", href: "/contact" },
  ];
</script>

<Header />
<Sidebar {navItems} />

<main>
  {#each people as person}
    <Card {person} />
  {/each}
</main>

<Footer />


<p>
  Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
</p>

<section>
  <Card />
  <Card />
</section>

<style>
</style>
