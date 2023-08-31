<footer>
  <h2>
    <a href="/">Alchemy</a>
  </h2>
  <div class="content">
    <section>
      <h4>Contact</h4>
      <a href="/contact">Contact Us</a>
    </section>
    <section>
      <h4>Legal</h4>
      <a href="/legal/tos">Terms of Service</a>
      <a href="/legal/privacy">Privacy Policy</a>
    </section>
  </div>
  <div class="small">Google Play and the Google Play logo are trademarks of Google LLC.</div>
</footer>

<style>
  .content {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
    flex-wrap: wrap;
  }

  .content > section {
    padding: 1rem;
    text-align: center;
  }

  .content > section > * {
    display: block;
  }

  .content h4 {
    color: white;
    margin: 0;
  }

  .small {
    font-size: 0.7rem;
    padding: 8px;
    text-align: center;
  }

  footer {
    background-color: black;
    color: white;
    font-size: 0.8rem;
    scroll-snap-align: start;
  }

  footer > h2 {
    margin: 0;
    padding: 1rem;
    text-align: center;
  }
</style>
