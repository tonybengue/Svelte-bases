<script>
  import { Link } from 'svelte-routing'

	import Header from '../components/Header.svelte'
	import Footer from '../components/Footer.svelte'

	let me = 'Tony'
</script>

<Header />
<main>
	<h1>Welcome on {me} website</h1>
  <Link to="blog">Blog</Link><br />
  <Link to="about">About</Link>
</main>
<Footer />

<style>
	p {
		color: purple;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}

	main {
		text-align: center;
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