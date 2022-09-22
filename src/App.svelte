<script>
  export let name;

  let mountains = '../public/mountains.jpg'
</script>

<main>
  <h1>Hello {name}!</h1>
  <h1>TJ Albertson</h1>
  <h3>FullStack Developer</h3>
  <hr />
  <div class="sites-flex">
    <div class="site" >
		<h2>Cloudbox</h2>
		<img {mountains}/>
  	</div>
    <div class="site" >
		<h2>The Colosseum</h2>
    	<img />
  	</div>
	</div>
	  <hr />
  <p>
    Contact Info + Links
  </p>
</main>

<style>
	p {
		display: flex;
		flex-direction: column	;
	}
  .site {
	  border-style: solid;
    margin: 15px;
  }

  .sites-flex {
    display: flex;
    align-items: center;
  justify-content: center;
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
