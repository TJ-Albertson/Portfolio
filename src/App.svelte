<script>
  import Cloudbox from "./SVG/Cloudbox.svelte";
  import Mail from "./SVG/Mail.svelte";
  import Rome from "./SVG/Rome.svelte"

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
      <div class="links">
        <a href="">Website</a> | <a href="">Github</a>
      </div>
    </div>
    <div class="site">
      <div class="site-header">
        <Rome />
        <h2>The Colosseum</h2>
      </div>

      <img src="images/nature.jpg" />
      <div class="links">
        <a href="">Website</a> | <a href="">Github</a>
      </div>
    </div>
  </div>
  <h2>Contact Me</h2>
  <div class="contact-footer">
    <Mail />
    <p>tj.albertson@outlook.com</p>
  </div>

  <div class="stripe" />
  <div class="background" />
</main>

<style>

  .colosseum {
    height: 50px;
    width: 50px;
  }

  .stripe {
    background-color: #ebf5fb;
    position: absolute;
    left: 50%;
    top: 50%;
    -webkit-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    height: 100vh;
    width: 60%;
    z-index: -3;
  }

  .background {
    background-color: #808b96;
    position: absolute;
    left: 50%;
    top: 50%;
    -webkit-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    height: 100vh;
    width: 100%;
    z-index: -4;
  }

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
    border-radius: 15px;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    z-index: 1;
    background: rgb(255, 255, 255);
  }

  .contact-footer {
    display: inline-flex;
    font-family: sans-serif;
    gap: 15px;
    align-items: center;
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
    margin-top: 0;
    margin-bottom: 0;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
