<script>
  export let navItems;
</script>

<aside>
  <nav>
    <ul>
      {#each navItems as item}
        <li><a href={item.href}>{item.text}</a></li>
      {/each}
    </ul>
  </nav>
</aside>

<style>
  aside {
    background: #f4f4f4;
    grid-column: 1 / 2;
    padding-right: 5em;
  }

  ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
  }

  li {
    list-style: none;
  }

  a {
    text-decoration: none;
    color: black;
  }

  a:hover {
    color: rebeccapurple;
  }
</style>
