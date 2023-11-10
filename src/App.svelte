<script>
  let files = null;

  function uploadImage() {
	  console.log("Upload image");
	  const fileInput = document.getElementById('file');
	  fileInput.click()

  }

</script>

<nav>
	<a href="/">home</a>
	<a on:click|preventDefault={uploadImage} href="/">upload</a>
	<input id="file" hide="true" accept="image/png, image/jpeg" bind:files  type="file" />

	

</nav>

<main>
	<h1>Welcome to Med-BlockChain</h1>
	<p>Visit the <a href="https://ayushksingh.com/">CEO's website </a> .</p>
	<p>The next generation of personal data storage is here...</p>
</main>

<style>
	#file {
      display: none;
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