<script lang="ts">
  const articles = [
    {
      date: "2024.12.16",
      category: "オフィス活用デザイン",
      title: "おしゃれなオフィスで社員のモチベーションもアップ！働きやすいオフィスデザインの事例を紹介",
      image: "https://images.unsplash.com/photo-1497366811353-6870744d04b2?q=80&w=2069&auto=format&fit=crop"
    },
    {
      date: "2024.12.02",
      category: "フリーアドレス",
      title: "フリーアドレスとは？導入のメリットや注意点、レイアウト事例を解説",
      image: "https://images.unsplash.com/photo-1524758631624-e2822e304c36?q=80&w=2070&auto=format&fit=crop"
    },
    {
      date: "2024.12.01",
      category: "オフィスづくりのコツ",
      title: "会社の固定席の幅、役職者にはどんな位置が適切？パターン別に解説",
      image: "https://images.unsplash.com/photo-1604328698692-f76ea9498e76?q=80&w=2070&auto=format&fit=crop"
    },
    {
      date: "2024.11.27",
      category: "オフィスづくりのコツ",
      title: "オフィスの一人あたり面積の目安は？快適なオフィスづくりに必要な広さと算出方法を解説",
      image: "https://images.unsplash.com/photo-1589829085413-56de8ae18c73?q=80&w=2112&auto=format&fit=crop"
    }
  ];
</script>

<section class="py-32 px-4 md:px-12 max-w-7xl mx-auto">
  <div class="flex justify-between items-end mb-16 border-b border-gray-200 pb-6">
    <h2 class="text-3xl font-light tracking-wide">Journal</h2>
    <a href="/journal" class="text-[10px] uppercase tracking-[0.2em] text-gray-400 hover:text-black transition-colors">See All</a>
  </div>

  <div class="flex flex-col">
    {#each articles as article}
      <a href="/journal/post" class="group flex flex-col md:flex-row gap-8 py-10 border-b border-gray-100 items-start hover:bg-gray-50 transition-colors px-4 -mx-4">
        <!-- Date & Category -->
        <div class="w-full md:w-1/4 pt-1">
          <div class="text-[10px] font-mono text-gray-400 mb-2 tracking-wide">{article.date}</div>
          <div class="text-[10px] text-gray-500 tracking-wide">{article.category}</div>
        </div>

        <!-- Title -->
        <div class="w-full md:w-1/2">
          <h3 class="text-base font-normal leading-relaxed text-gray-800 group-hover:text-gray-600 transition-colors tracking-wide">
            {article.title}
          </h3>
        </div>

        <!-- Thumbnail -->
        <div class="w-full md:w-1/4 flex justify-end">
          <div class="w-32 h-20 overflow-hidden bg-gray-200">
            <img src={article.image} alt="" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" />
          </div>
        </div>
      </a>
    {/each}
  </div>
</section>
