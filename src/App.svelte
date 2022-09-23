<script>
  import Cloudbox from "./SVG/Cloudbox.svelte";
  import Mail from "./SVG/Mail.svelte";
  import Rome from "./SVG/Rome.svelte";
</script>

<main>
  <head>
    <script
      src="https://kit.fontawesome.com/4cc35cc184.js"
      crossorigin="anonymous"></script>
  </head>

  <table>
    <tr>
      <td class="animated zoomIn" style="animation-delay:2.2s;"
        ><a class="social"><i class="fab fa-facebook" /></a></td
      >
      <td class="animated zoomIn" style="animation-delay:2.4s;"
        ><a class="social"><i class="fab fa-twitter" /></a></td
      >
      <td class="animated zoomIn" style="animation-delay:2.6s;"
        ><a class="social"><i class="fab fa-instagram" /></a></td
      >
      <td class="animated zoomIn" style="animation-delay:2.8s;"
        ><a class="social"><i class="fab fa-dribbble" /></a></td
      >
      <td class="animated zoomIn" style="animation-delay:3.0s;"
        ><a class="social"><i class="fab fa-medium" /></a></td
      >
    </tr>
  </table>
  <h1>TJ Albertson</h1>
  <h3>Fullstack Developer</h3>

  <h1>Projects</h1>
  

  <div class="sites-flex">
    <div class="site">
      <div class="site-header">
        <Cloudbox />
        <h2>Cloudbox</h2>
      </div>

      <img src="images/mountains.jpg" />
      <div class="links">
        <a href="">Demo</a> | <a href="">Github</a>
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
  @import url("https://fonts.googleapis.com/css?family=Poppins");

  .social {
    color: rgb(255, 44, 90);
    font-size: 23px;
    padding: 12px 17px;
    border-radius: 50%;
    background: transparent;
    transition: 0.4s ease-in-out;
    font-weight: bold;
    margin: 0px 8px;
  }

  .social:hover {
    cursor: pointer;
    color: #fff;
    background: rgb(255, 44, 90);
    box-shadow: 0px 10px 30px rgba(255, 66, 107, 0.8);
  }

  .colosseum {
    height: 50px;
    width: 50px;
  }

  .table {
    justify-content: center;
  }

  .stripe {
    background-color: #ffffff;
    position: absolute;
    left: 50%;
    top: 50%;
    -webkit-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    height: 100vh;
    width: 100%;
    z-index: -3;
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
    transition: 0.4s ease-in-out;
  }

  .site:hover {
    transform: scale(1.03);
    cursor: pointer;
    box-shadow: 0 16px 32px 0 rgba(0, 0, 0, 0.2),
      0 6px 20px 0 rgba(0, 0, 0, 0.19);
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
    font-size: 2em;
    font-weight: 100;
    font-family: "Poppins", sans-serif;
    margin-top: 0;
    margin-bottom: 0;
    padding-top: 35px;
  }

  h3 {
    margin: 0px;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
