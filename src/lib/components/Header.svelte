<script lang="ts">
  import { onMount } from 'svelte';

  export let transparent = false;
  
  let isScrolled = false;

  onMount(() => {
    const handleScroll = () => {
      isScrolled = window.scrollY > 50;
    };
    
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  });
</script>

<header 
  class="fixed top-0 left-0 w-full z-50 px-8 py-8 flex justify-between items-start text-[10px] font-medium tracking-[0.15em] uppercase transition-all duration-500 
  {isScrolled ? 'bg-white/90 backdrop-blur-md text-gray-900 py-4 shadow-sm' : (transparent ? 'text-white' : 'text-gray-900')}"
>
  <!-- Left Side (Empty/Hidden) -->
  <div class="w-24 hidden md:block">
      <!-- Placeholder for spacing -->
  </div>

  <!-- Center Navigation -->
  <nav class="flex-1 flex justify-center space-x-8 md:space-x-12">
    <a href="/" class="hover:opacity-60 transition-opacity">Home</a>
    <a href="/works" class="hover:opacity-60 transition-opacity">Works</a>
    <a href="/about" class="hover:opacity-60 transition-opacity">About</a>
    <a href="/journal" class="hover:opacity-60 transition-opacity">Journal</a>
    <a href="/company" class="hover:opacity-60 transition-opacity">Company</a>
    <a href="/designers" class="hover:opacity-60 transition-opacity">Designers</a>
  </nav>

  <!-- Right Side -->
  <div class="w-24 flex justify-end">
    <a href="/contact" class="hover:opacity-60 transition-opacity">Contact</a>
  </div>
</header>
