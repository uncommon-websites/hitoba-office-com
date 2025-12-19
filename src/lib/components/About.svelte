<script lang="ts">
  const aboutImage = "https://images.unsplash.com/photo-1497215728101-856f4ea42174?q=80&w=2070&auto=format&fit=crop";
  const smallImage = "https://images.unsplash.com/photo-1664575602554-2087b04935a5?q=80&w=2574&auto=format&fit=crop"; // Hands working
</script>

<section class="bg-[#EAEAE6] min-h-screen flex flex-col md:flex-row">
  <!-- Left Content -->
  <div class="w-full md:w-1/2 p-12 md:p-24 lg:p-32 flex flex-col justify-center relative">
    <span class="text-[10px] uppercase tracking-[0.2em] mb-16 block text-gray-500">[About]</span>
    
    <div class="max-w-md relative z-10">
      <h3 class="text-lg leading-loose font-normal mb-8 text-gray-900 tracking-wide">
        WORKKITは、空間デザインを手がける「ヒトバデザイン」による、働く人と場をクライアントとともに豊かにしていく「共創プロジェクト」です。
      </h3>
      
      <p class="text-xs text-gray-500 mb-16 leading-loose tracking-wide">
        WORKKIT is a "co-creation project" by Hitoba Design, which handles spatial design, to enrich working people and places together with clients.
      </p>

      <div class="mb-16">
        <img src={smallImage} alt="Craftsmanship" class="w-40 h-56 object-cover shadow-xl" />
      </div>

      <a href="/about" class="inline-flex items-center justify-center px-10 py-3 border border-gray-400 rounded-full text-[10px] uppercase tracking-[0.2em] hover:bg-black hover:text-white hover:border-black transition-all duration-300">
        About Project
      </a>
    </div>
  </div>

  <!-- Right Image -->
  <div class="w-full md:w-1/2 h-[50vh] md:h-auto relative">
    <img src={aboutImage} alt="Office Environment" class="w-full h-full object-cover" />
  </div>
</section>
