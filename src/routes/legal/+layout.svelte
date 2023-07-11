<script>
  import Footer from "../Footer.svelte";
  import HeroIcon from "../HeroIcon.svelte";
</script>

<main class="tos">
  <HeroIcon />
  <slot />
</main>
<Footer />

<style>
  main.tos {
    font-weight: lighter;
    font-size: 12pt;
    line-height: 1.5;
    margin: 5rem auto;
    max-width: 60ch;
    min-height: calc(100vh - 5rem);
    text-align: justify;
  }

  main.tos :global(h1) {
    text-align: center;
  }

  main.tos :global(h2),
  main.tos :global(h3) {
    text-align: left;
  }
</style>
