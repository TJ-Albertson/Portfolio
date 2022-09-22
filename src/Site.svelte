<script>
    import Icon from './Icon.svelte';
  </script>
  
  <main>
      <div class="site">
        <h2><Icon name="cloudbox" />Cloudbox</h2>
        <img src="images/mountains.jpg" />
        <p>Repositories</p>
        <hr />
        <div class="links">
          <a href="">Cloudbox</a> | <a href="">API</a> |
          <a href="">Logs</a>
        </div>
      </div>
  </main>
  
  <style>
    .links {
      margin-bottom: 15px;
    }
  
    .site {
      border-style: solid;
      margin: 25px;
      margin-left: 55px; 
      margin-right: 55px; 
    }
  
    main {
      text-align: center;
      padding: 1em;
      max-width: 240px;
      margin: 0 auto;
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