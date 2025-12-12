<script lang="ts">
  const cards = [
    {
      title: "We Don't Optimize for Engagement...",
      subtitle: "We Optimize for Correctness.",
      image: ""
    },
    {
      title: "We Don't Extract Attention...",
      subtitle: "We Protect Your Dignity.",
      image: ""
    },
    {
      title: "We Don't Build Feeds...",
      subtitle: "We Ground You in Reality.",
      image: ""
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      Modern platforms failed because they severed human connection from physical reality. Seven Degrees brings it back—with restraint, ethics, and architectural integrity.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card, i}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-50 border border-gray-200 flex items-center justify-center">
          <span class="text-6xl font-bold text-gray-200">{i + 1}</span>
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>0{i + 1}</span>
           <span>→</span>
        </div>
      </div>
    {/each}
  </div>
</section>
