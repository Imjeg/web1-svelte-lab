<script>
  export let data;
  import Card from "../components/Card.svelte";
  const people = data.people;
  console.log(people);
</script>

<main>
{#each people as  person}
  <Card {person} />
{/each}
</main>

<style>
  main {
    background: white;
    display: flex;
    flex-wrap: wrap;
    gap: 2em;
  }
</style>