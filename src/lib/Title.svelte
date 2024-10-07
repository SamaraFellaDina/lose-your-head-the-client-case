<script>
  import Icon from "./Icon.svelte";
  export let company = data.sites;
  export let resultsheet = data.scans;
</script>

<section class="title">
  <article>
    <p>Automatische Scan</p>
    <h1>{company[0].title}/home</h1>
  </article>
  <nav>
    <button><Icon name="arrow-left" /></button>
    <!-- <span><p>{resultsheet[0].date}</p></span> -->
     <span>Aug.</span>
    <button><Icon name="arrow-right" /></button>
  </nav>
</section>

<style>

  section {
    padding-top: var(--average-padding);
    grid-area: 1 / 1 / 2 / 3;
    display: flex;
    justify-content: space-between;
  }

  h1 {
    font-size: 2em;
  }

  nav {
    display: flex;
    align-items: center;
    gap: 10px;
  }

  button {
    background-color: var(--color-background-section);
    border-radius: var(--section-border-radius);
    box-shadow: var(--box-shadow);
    padding: 10px 20px;
  }

  span {
    background-color: var(--color-background-section);
    border-radius: var(--section-border-radius);
    box-shadow: var(--box-shadow);
    padding: 10px 20px;
  }

</style>