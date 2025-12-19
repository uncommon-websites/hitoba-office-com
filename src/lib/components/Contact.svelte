<script lang="ts">
  const contactBg = "https://images.unsplash.com/photo-1504384308090-c54be3855833?q=80&w=2574&auto=format&fit=crop";
  const contactInset = "https://images.unsplash.com/photo-1517245386807-bb43f82c33c4?q=80&w=2070&auto=format&fit=crop";
</script>

<section class="relative py-32 px-4 md:px-12 min-h-[90vh] flex items-center justify-center overflow-hidden">
  <!-- Background Parallax-ish -->
  <div class="absolute inset-0 z-0">
    <img src={contactBg} alt="Office" class="w-full h-full object-cover opacity-90" />
  </div>

  <!-- Card -->
  <div class="relative z-10 bg-[#EAEAE6] p-8 md:p-16 max-w-5xl w-full shadow-2xl flex flex-col md:flex-row gap-16 items-center">
    
    <div class="flex-1 py-8">
      <h2 class="text-5xl md:text-6xl font-light mb-16 tracking-tight">Contact</h2>
      
      <p class="text-sm text-gray-800 leading-loose mb-8 tracking-wide">
        お仕事や協業のご相談、採用のご応募は<br>
        こちらよりお願いいたします。
      </p>
      
      <p class="text-[10px] text-gray-400 mb-16 leading-relaxed tracking-wide">
        For inquiries about work, collaboration, or recruitment,<br>
        please contact us here.
      </p>

      <a href="/contact" class="group inline-flex items-center gap-6 text-[10px] uppercase tracking-[0.2em] hover:opacity-60 transition-opacity">
        <span class="w-12 h-12 rounded-full border border-black flex items-center justify-center group-hover:bg-black group-hover:text-white transition-colors">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round">
            <path d="M5 12h14M12 5l7 7-7 7"/>
          </svg>
        </span>
      </a>
    </div>

    <div class="w-full md:w-72 aspect-[3/4] relative">
      <img src={contactInset} alt="Contact" class="w-full h-full object-cover grayscale opacity-90" />
    </div>

  </div>
</section>
