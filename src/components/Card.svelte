<script>
  export let person;
  import Picture from "./Picture.svelte";
  import Details from "./Details.svelte";
</script>

<section>
  <Picture {person} />
  <Details {person} />
</section>

<style>
  section {
    display: flex;
    border: 1px solid black;
    padding: 1.5em;
    gap: 1em;
    width: 400px;
    grid-column: 2/3;
  }
</style>
