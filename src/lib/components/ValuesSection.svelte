<script lang="ts">
  const photos = [
    {
      title: "Campus Life",
      desc: "Meet classmates between lectures, discover study partners in the library, connect at campus events. Seven Degrees turns your campus into a network.",
      img: ""
    },
    {
      title: "Coffee Shops & Cafés",
      desc: "That person working across from you? They might be the co-founder you've been looking for. Proximity creates serendipity.",
      img: ""
    },
    {
      title: "Events & Gatherings",
      desc: "Conferences, concerts, meetups. Dense environments where meaningful connections happen. Seven Degrees makes them intentional.",
      img: ""
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">Built for real-world environments.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      Seven Degrees isn't just another app—it's a human adjacency layer for dense physical spaces. Meet people where you already are, without the noise of endless swiping.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each photos as photo}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-50 border border-gray-200 flex items-center justify-center p-6">
          <span class="text-sm text-gray-400 text-center">{photo.title}</span>
        </div>
        <h4 class="text-xs font-bold mb-1">{photo.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{photo.desc}</p>
      </div>
    {/each}
  </div>
</section>
