<svelte:head>
  <title>Alchemy</title>
</svelte:head>

<slot />

<style>
  :global(:root) {
    --background-color: #fff;
    --text-color: #222;
    --subtitle-color: #555;
    --primary-color: #7cff66;
    --secondary-color: #00d2fc;
    --error-color: #f50000;
  }

  :global(a) {
    color: var(--secondary-color);
    text-decoration: none;
  }

  :global(body) {
    background-color: var(--background-color);
    color: var(--text-color);
    font-family: "Lexend", sans-serif;
    margin: 0;
    padding: 0;
  }

  :global(button) {
    background-color: var(--primary-color);
    border: none;
    border-radius: 16px;
    font-family: "Lexend", sans-serif;
    font-weight: bold;
    padding: 8px 24px;
  }

  :global(dialog) {
    border: none;
    border-radius: 16px;
    padding: 16px;
  }

  :global(dialog::backdrop) {
    backdrop-filter: blur(4px);
  }

  :global(h1, h2, h3) {
    color: var(--text-color);
  }

  :global(h4, h5, h6) {
    color: var(--subtitle-color);
  }

  :global(main) {
    padding: 16px;
  }
</style>
