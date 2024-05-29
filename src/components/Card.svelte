<script>
  import Picture from "./Picture.svelte";
  import Details from "./Details.svelte";
  export let person;
</script>

<section>
  <Picture {person}/>
  <Details {person} />
</section>

<style>
  section {
      width: 400px;
      background-color: white;
      display: flex;
      border: 1px solid black;
      padding: 1.5em;
      gap: 1em;
      grid-column: 2/3;
  }
</style>
