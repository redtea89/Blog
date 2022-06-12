<script>
	import Header from "./components/Header.svelte"
	import Nav from "./components/Nav.svelte"
	import Section02 from "./components/Section02.svelte"
	import Footer from "./components/Footer.svelte"
</script>

<header>
	<Header />
</header>
<nav>
	<Nav />
</nav>
<main>
	<Section02 />
</main>
<footer>
	<Footer />
</footer>

<style>
	header {
		text-align: center;
		margin: 0 auto;
	}

	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}

	/* @media (min-width: 640px) {
		main {
			max-width: none;
		}
	} */
</style>