<script>
  import Cloudbox from "./SVG/cloudbox.svelte";
</script>

<main>
  <h1>TJ Albertson</h1>
  <h2>Fullstack Developer</h2>

  <div class="sites-flex">
    <div class="site">
      <div class="site-header">
        <Cloudbox />
        <h2>Cloudbox</h2>
      </div>

      <img src="images/mountains.jpg" />
      <p>Repositories</p>
      <hr />
      <div class="links">
        <a href="">Cloudbox</a> | <a href="">API</a> |
        <a href="">Logs</a>
      </div>
    </div>
    <div class="site">
      <div class="site-header">
        <Cloudbox />
        <h2>The Colosseum</h2>
      </div>

      <img src="images/nature.jpg" />
      <p>Repositories</p>
      <hr />
      <div class="links">
        <a href="">The Colosseum</a> | <a href="">Logs</a>
      </div>
    </div>
  </div>
  <hr />
  <p>Contact Info + Links</p>
</main>

<style>
  

  .links {
    margin-bottom: 15px;
  }

  img {
    height: 350px;
    width: 700px;
    margin: 15px;
  }

  p {
    margin: 0px;
  }

  .site {
    margin: 25px;
    margin-left: 55px;
    margin-right: 55px;
    width: 50rem;
    background: white;
    border-radius: 15px;
  }

  .site-header {
    display: inline-flex;
    font-family: sans-serif;
    font-size: 40px;
    margin: 15px;
    gap: 15px;
    align-items: center;
    height: 80px;
  }

  .sites-flex {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #EBF5FB;
  }

  main {
    text-align: center;
    padding: 0;
    max-width: 240px;
    margin: 0;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
