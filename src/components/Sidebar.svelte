<script>
  export let navItems;
</script>

<aside>
<nav>
  <ul>
    {#each navItems as Item}
      <li><a href={Item.href}>{Item.text}</a></li>
    {/each}
  </ul>
</nav>
</aside>

<style>
aside{
  background: lightblue;
  grid-column: 1 / 2;
  padding-right: 5em;
}
</style>