<script lang="ts">
  const features = [
    {
      title: "Proximity Discovery",
      desc: "Discover people nearby using device-level proximity signals. Physical presence becomes the foundation of connection.",
      bg: "bg-black",
      img: "",
      dark: true
    },
    {
      title: "Two-Stage Reveal",
      desc: "Stage 1 shows visual presence only. Stage 2 provides full reveal after mutual interest. No coercion, complete psychological safety.",
      bg: "bg-gray-100",
      img: "",
      dark: false
    },
    {
      title: "Offline-First Messaging",
      desc: "Core system works without internet. Encrypted mesh messaging with deferred sync. The cloud accelerates, but never owns your data.",
      bg: "bg-primary-950",
      img: "",
      dark: true
    },
    {
      title: "Privacy Invariants",
      desc: "On-device processing, encrypted local vaults, minimal server knowledge. Irreversible 'Vaporize' exits with cryptographic guarantees.",
      bg: "bg-gray-100",
      img: "",
      dark: false
    },
    {
      title: "Calm Technology",
      desc: "No feeds, no infinite scroll, no engagement dark patterns. Designed to feel still with immediate load and motion only when meaningful.",
      bg: "bg-gray-100",
      img: "",
      dark: false,
      full: true
    },
    {
      title: "Mutual Intent",
      desc: "Nothing happens without reciprocal consent. Optimizing for correct moments, not time spent.",
      bg: "bg-gray-100",
      img: "",
      dark: false
    },
    {
      title: "Real-World Grounding",
      desc: "Not another abstract feed. A human adjacency layer for dense environments: campuses, cafés, offices, events, cities.",
      bg: "bg-gray-100",
      img: "",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">Built on architectural principles</span> that prioritize your privacy, dignity, and real-world connections over engagement metrics and manipulation.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each features as feature}
      <div class="group {feature.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${feature.bg} mb-4 ${feature.full ? 'md:aspect-[2.5/1]' : ''} flex items-center justify-center p-8`}>
          <div class="text-center">
            <span class={`text-3xl md:text-4xl font-bold ${feature.dark ? 'text-white' : 'text-black'}`}>{feature.title}</span>
          </div>
        </div>
        <h3 class="text-sm font-bold mb-1">{feature.title}</h3>
        <p class="text-sm text-gray-600">{feature.desc}</p>
      </div>
    {/each}
  </div>
</section>
