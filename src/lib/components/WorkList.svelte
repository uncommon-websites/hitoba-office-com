<script lang="ts">
  const projects = [
    {
      title: "FUJIMOTO INC.",
      image: "https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?q=80&w=2070&auto=format&fit=crop",
      area: "660㎡ / 200t",
      completion: "2023",
      tags: ["Renovation", "Office"],
      client: "FUJIMOTO INC."
    },
    {
      title: "e-dash Co., Ltd.",
      image: "https://images.unsplash.com/photo-1600607686527-6fb886090705?q=80&w=2000&auto=format&fit=crop",
      area: "396㎡ / 120t",
      completion: "2024",
      tags: ["Office", "Interior"],
      client: "e-dash Co., Ltd."
    },
    {
      title: "Atrae, Inc. vol.4",
      image: "https://images.unsplash.com/photo-1534438327276-14e5300c3a48?q=80&w=2070&auto=format&fit=crop",
      area: "396㎡ / 120t",
      completion: "2024",
      tags: ["Office", "Gym"],
      client: "Atrae, Inc."
    },
    {
      title: "Open Group Inc.",
      image: "https://images.unsplash.com/photo-1556761175-5973dc0f32e7?q=80&w=2664&auto=format&fit=crop",
      area: "1650㎡ / 499t",
      completion: "2024",
      tags: ["Office", "Lounge"],
      client: "Open Group Inc."
    },
    {
      title: "WORKKIT",
      image: "https://images.unsplash.com/photo-1555664424-778a1e5e1b48?q=80&w=2070&auto=format&fit=crop", // Futuristic server room vibe
      area: "1650㎡ / 499t",
      completion: "2024",
      tags: ["Branding", "Office"],
      client: "WORKKIT Corporation"
    }
  ];
</script>

<section class="py-20 px-4 md:px-12 max-w-7xl mx-auto">
  <div class="flex flex-col gap-32">
    {#each projects as project}
      <div class="group cursor-pointer">
        <!-- Image Container -->
        <div class="w-full aspect-[16/9] overflow-hidden mb-6 bg-gray-100">
          <img 
            src={project.image} 
            alt={project.title} 
            class="w-full h-full object-cover transition-transform duration-1000 group-hover:scale-105"
          />
        </div>

        <!-- Project Details -->
        <div class="grid grid-cols-1 md:grid-cols-12 gap-4 text-sm pt-2">
          <!-- Title -->
          <div class="md:col-span-4 font-normal text-base tracking-wide">{project.title}</div>
          
          <!-- Meta -->
          <div class="md:col-span-4 flex flex-col md:flex-row gap-8 md:gap-16 text-gray-800 text-xs">
            <div>
              <span class="block text-gray-400 text-[10px] uppercase tracking-wider mb-1">Area</span>
              {project.area}
            </div>
            <div>
              <span class="block text-gray-400 text-[10px] uppercase tracking-wider mb-1">Completion</span>
              {project.completion}
            </div>
          </div>

          <!-- Tags -->
          <div class="md:col-span-4 text-right text-gray-500 text-[10px] uppercase tracking-widest">
            {project.tags.join(" / ")}
          </div>
        </div>
      </div>
    {/each}
  </div>

  <div class="mt-40 text-center">
    <a href="/works" class="inline-block text-xl font-light border-b border-black pb-1 hover:opacity-60 transition-opacity">See All Works</a>
  </div>
</section>
