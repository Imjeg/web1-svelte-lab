<script>
  export let navItems;
</script>

<header>
  <h1>Welcome to SvelteKit</h1>
  <nav>
    <ul>
      {#each navItems as item}
        <li><a href={item.href}>{item.text}</a></li>
      {/each}
    </ul>
  </nav>
</header>

<style>
  header {
    background-color: rebeccapurple;
  }
</style>