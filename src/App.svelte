<script>
	import Header from "./components/Header.svelte";
	import Intro from "./components/Intro.svelte";
	import Pricing from "./components/Pricing.svelte";
	import Topics from "./components/Topics.svelte";
	import Reviews from "./components/Reviews.svelte";
	import Contact from "./components/Contact.svelte";
	import Footer from "./components/Footer.svelte";
</script>

<main>
	<Header />

	<section id="intro">
		<Intro />
	</section>

	<section id="pricing" class="bg-light mt-5">
		<Pricing />
	</section>

	<section id="topics">
		<Topics />
	</section>

	<section id="reviews" class="bg-light">
		<Reviews />
	</section>

	<section id="contact">
		<Contact />
	</section>

	<section class="bg-light">
		<Footer on:click />
	</section>
</main>

<style>
	section {
		padding: 60px 0;
	}
</style>
