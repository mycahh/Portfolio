<script>
	import Header from './components/Header.svelte'
	import Navbar from './components/Navbar.svelte'
	import Hero from './components/Hero.svelte'

	import Projects from './components/Projects.svelte'
	import Project from './components/Project.svelte'
	import About from './components/About.svelte'
	import Contact from './components/Contact.svelte'
	import Footer from './components/Footer.svelte'
</script>

<Header>
	<Navbar />
	<Hero />
</Header>
<Projects>
	<Project />
	<Project reverse={true}/>
	<Project />
</Projects>
<About />
<Contact />
<Footer />

<style>
	:global(body) {
		font-size: 12px;
	}

	@media(min-width: 767px) {
		:global(body) {
			font-size: 14px;
		}
	}

	@media(min-width: 1024px) {
		:global(body) {
			font-size: 16px;
		}
	}
</style>