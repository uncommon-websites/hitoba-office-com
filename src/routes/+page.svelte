<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import WorkList from "$lib/components/WorkList.svelte";
  import About from "$lib/components/About.svelte";
  import Journal from "$lib/components/Journal.svelte";
  import Contact from "$lib/components/Contact.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<main class="w-full overflow-x-hidden bg-white">
  <Header transparent={true} />
  <Hero />
  <WorkList />
  <About />
  <Journal />
  <Contact />
  <Footer />
</main>

