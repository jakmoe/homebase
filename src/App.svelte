<script lang="ts">
	import Footer from "./components/Footer.svelte";
	import Navbar from "./components/Navbar.svelte";
	export let name: string;
</script>

<main>
	<Navbar/>

	<section class="section">
		<div class="container">
			<h1 class="title">
				Hello {name}
			</h1>
			<p class="subtitle">
				My first website with <strong>Bulma</strong>!
			</p>
		</div>
	</section>

	<Footer/>
</main>

<style lang="scss">
	@import "base";
	@import "../node_modules/bulma/sass/elements/container.sass";
	@import "../node_modules/bulma/sass/layout/section.sass";
	@import "../node_modules/bulma/sass/elements/title.sass";

	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>