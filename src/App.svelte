<script>
  import Cloudbox from "./SVG/Cloudbox.svelte";
  import Mail from "./SVG/Mail.svelte";
  import Rome from "./SVG/Rome.svelte";
  import Paint_Colosseum from "./SVG/Paint_Colosseum.svelte";
  import Paint_Cloudbox from "./SVG/Paint_Cloudbox.svelte";
  import PaintSplat_Colosseum from "./SVG/PaintSplat_Colosseum.svelte";
  import PaintSplat_Cloudbox from "./SVG/PaintSplat_Cloudbox.svelte";
</script>

<main>
  <head>
    <script
      src="https://kit.fontawesome.com/4cc35cc184.js"
      crossorigin="anonymous"></script>
  </head>

  <h1>TJ Albertson</h1>
  <h3>Fullstack Developer</h3>
  <table>
    <tr>
      <td class="animated zoomIn" style="animation-delay:2.2s;"
        ><a
          class="social"
          href="https://github.com/TJ-Albertson"
          target="_blank"><i class="fa-brands fa-github" /></a
        ></td
      >
      <td class="animated zoomIn" style="animation-delay:2.4s;"
        ><a
          class="social"
          href="https://linkedin.com/in/thomas-albertson-895443250"
          target="_blank"><i class="fa-brands fa-linkedin" /></a
        ></td
      >
      <td class="animated zoomIn" style="animation-delay:2.6s;"
        ><a
          class="social"
          href="./images/resume.pdf"
          target="_blank"
          alt="resume"><i class="fa-regular fa-file" /></a
        ></td
      >
    </tr>
  </table>
  <h2 class="contact">Projects</h2>

  <div class="flex-container">
    <div class="flex-item">
      <div class="paint-cloudbox">
        <Paint_Cloudbox />
      </div>

      <div class="site-card">
        <div class="paint-splat-cloudbox">
          <PaintSplat_Cloudbox />
        </div>

        <div class="site-header" id="cloudbox">
          <Cloudbox />
          <h2>Cloudbox</h2>
        </div>

        <img src="images/cloudbox.png" alt="colosseum-preview" />
        <div class="links">
          <a href="http://cloud-box-storage.com">Demo</a> |
          <a href="https://github.com/TJ-Albertson/Cloudbox" target="_blank"
            >Github</a
          >
        </div>
      </div>
    </div>

    <div class="flex-item">
      <div class="paint-colosseum">
        <Paint_Colosseum />
      </div>

      <div class="site-card">
        <div class="paint-splat-colosseum">
          <PaintSplat_Colosseum />
        </div>

        <div class="site-header" id="colosseum">
          <Rome />
          <h2>The Colosseum</h2>
        </div>

        <img src="images/colosseum.png" alt="colosseum-preview" />
        <div class="links">
          <a href="http://themoviecolosseum.com">Website</a> |
          <a
            href="https://github.com/TJ-Albertson/The-Colosseum"
            target="_blank">Github</a
          >
        </div>
      </div>
    </div>
  </div>
  <h2 class="contact ">Contact Me</h2>
  <div class="contact-footer">
    <Mail /> tj.albertson@outlook.com
  </div>
</main>

<style>
  @import url("https://fonts.googleapis.com/css?family=Poppins");

  main {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    padding: 0;
    margin: 0;
    overflow: hidden;
  }

  h1 {
    color: rgb(255, 44, 90);
    font-size: 3em;
    font-weight: 100;
    font-family: "Poppins", sans-serif;
    margin-top: 0;
    margin-bottom: 0;
    padding-top: 35px;
  }

  h3 {
    margin: 0px;
    margin-bottom: 15px;
  }

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

  .contact {
    padding: 5px 0px;
    border-bottom: 4px solid rgb(255, 44, 90);
    width: auto;
  }
  /*        */
  .flex-container {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .flex-item {
    position: relative;
    margin: 25px;
    margin-left: 55px;
    margin-right: 55px;
    width: 50rem;
  }
  .site-card {
    border-radius: 15px;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    transition: 0.4s ease-in-out;
    background-color: #fff;
    position: relative;
    z-index: 1;
  }

  .site-card:hover {
    transform: scale(1.03);
    cursor: pointer;
    box-shadow: 0 16px 32px 0 rgba(0, 0, 0, 0.2),
      0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }
  /*        */
  .site-header {
    display: inline-flex;

    font-size: 40px;
    margin: 15px;
    gap: 15px;
    align-items: center;
    height: 80px;
  }

  #cloudbox {
    font-family: sans-serif;
  }

  #colosseum {
    font-family: "Open Sans";
    font-weight: bold;
  }

  img {
    width: 640px;
    height: 360px;
    margin: 10px;
    border-style: solid;
    border-color: grey;
  }

  .paint-splat-colosseum {
    position: absolute;
    top: 0;
    right: 0;
  }

  .paint-splat-cloudbox {
    position: absolute;
    bottom: 0;
    left: 0;
  }

  .paint-colosseum {
    position: absolute;
    top: -427.5px;
    right: -375px;
    z-index: 0;
  }

  .paint-cloudbox {
    position: absolute;
    bottom: -603.5px;
    left: -635px;
    z-index: 0;
  }

  a {
    color: rgb(255, 44, 90);
  }

  .links {
    margin-bottom: 15px;
  }
  /*        */

  /*        */
  .contact-footer {
    display: inline-flex;
    font-family: sans-serif;
    font-weight: bold;
    gap: 15px;
    align-items: center;
    margin-bottom: 30px;
  }

  @media only screen and (max-width: 640px) {
    .site {
      width: 5rem;
    }

    img {
      width: 16px;
      height: 9px;
    }

    .site-header {
      font-size: 10px;
      height: 40px;
    }

    .site-header-two {
      font-size: 10px;
      height: 40px;
    }

    .site-paint-one {
      visibility: hidden;
    }
  }

  @media only screen and (max-width: 840px) {
    .site {
      width: 35rem;
      margin: 20px;
    }

    img {
      width: 426px;
      height: 240px;
    }

    .site-header {
      font-size: 30px;
      height: 80px;
    }

    .site-header-two {
      font-size: 30px;
      height: 80px;
    }

    .site-paint-one {
      visibility: hidden;
    }
  }

  @media (orientation: portrait) {
    .sites-flex {
      flex-direction: column-reverse;
    }
    .stripe {
      top: 17em;
    }
  }
</style>
