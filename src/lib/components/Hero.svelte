<script lang="ts">
  // Placeholder image for the hero
  const heroImage = "https://images.unsplash.com/photo-1497366216548-37526070297c?q=80&w=2301&auto=format&fit=crop";
</script>

<section class="relative w-full h-screen overflow-hidden bg-gray-900 text-white">
  <!-- Background Image -->
  <div class="absolute inset-0 pl-16 md:pl-24">
    <img src={heroImage} alt="Office Interior" class="w-full h-full object-cover opacity-90" />
  </div>

  <!-- Left Sidebar (Solid Black/Dark) -->
  <div class="absolute top-0 left-0 h-full w-16 md:w-24 bg-[#111] z-20 flex flex-col justify-between items-center py-12">
    <!-- Counter -->
    <div class="text-[10px] font-mono tracking-widest mt-20">
      <span class="block">02</span>
      <span class="block w-full h-px bg-white/30 my-1"></span>
      <span class="block opacity-50">05</span>
    </div>
    
    <!-- Vertical Text Logo -->
    <div class="flex-1 flex items-center justify-center relative w-full">
       <h1 class="absolute whitespace-nowrap text-4xl md:text-5xl font-bold tracking-tighter -rotate-90 origin-center opacity-100 text-white">
         WORKKIT Corporation
       </h1>
    </div>

    <!-- Scroll Line -->
    <div class="mb-8 h-24 w-px bg-white/20 relative overflow-hidden">
        <div class="absolute top-0 left-0 w-full h-1/2 bg-white animate-pulses"></div>
    </div>
  </div>

  <!-- Content Overlay -->
  <div class="absolute bottom-0 left-0 w-full pl-24 md:pl-32 pr-8 md:pr-12 pb-12 flex flex-col md:flex-row justify-between items-end z-10">
    
    <!-- Left Bottom Info -->
    <div class="mb-8 md:mb-0 max-w-md">
        <h2 class="text-3xl md:text-4xl font-light leading-tight mb-3">FUJIMOTO INC.</h2>
        <div class="flex items-center gap-4 text-xs tracking-widest uppercase opacity-80">
            <span>Renovation</span>
            <span class="w-1 h-1 bg-white rounded-full"></span>
            <span>Office</span>
        </div>
    </div>

    <!-- Right Bottom Action & Info -->
    <div class="flex flex-col items-end text-right gap-12">
        
        <a href="/works/detail" class="group flex flex-col items-center gap-2 text-[10px] uppercase tracking-[0.2em] hover:opacity-80 transition-opacity">
            See Work Detail
            <span class="w-10 h-10 rounded-full border border-white/30 flex items-center justify-center group-hover:bg-white group-hover:text-black transition-all duration-300 backdrop-blur-sm">
                <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <path d="M12 5v14M19 12l-7 7-7-7"/>
                </svg>
            </span>
        </a>
        
        <div class="flex gap-12 text-[10px] tracking-widest">
            <div class="text-left">
                <span class="block opacity-40 mb-1">Area</span>
                1250㎡ / 378t
            </div>
            <div class="text-left">
                <span class="block opacity-40 mb-1">Completion</span>
                2024
            </div>
            <div class="text-left">
                 <span class="block opacity-40 mb-1">Client</span>
                 Fujimoto Inc.
            </div>
        </div>
    </div>
  </div>
</section>
