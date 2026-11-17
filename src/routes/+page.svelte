<script lang="ts">
  import Header from '$lib/components/sections/Header.svelte';
  import Hero from '$lib/components/sections/Hero.svelte';
  import Services from '$lib/components/sections/Services.svelte';
  import About from '$lib/components/sections/About.svelte';
  import Contact from '$lib/components/sections/Contact.svelte';
  import Footer from '$lib/components/sections/Footer.svelte';
</script>

<svelte:head>
  <title>Délice Diet | Cabinet de nutrition et de diététique</title>
  <meta name="description" content="Délice Diet, cabinet de nutrition et de diététique au Cameroun. Découvrez l’approche du cabinet et ses prestations." />
</svelte:head>

<a class="skip-link" href="#accueil">Aller au contenu</a>
<Header />
<main id="accueil" tabindex="-1">
  <Hero />
  <Services />
  <About />
  <Contact />
</main>
<Footer />
