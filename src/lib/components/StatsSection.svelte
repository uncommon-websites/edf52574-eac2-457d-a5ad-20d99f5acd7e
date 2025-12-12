<script lang="ts">
  const stats = [
    {
      label: "Offline-First",
      desc: "Core system works without internet for discovery, mutual signaling, matching, and messaging via encrypted mesh with deferred sync. Cloud accelerates experience but never owns it. Makes the system resilient and censorship-resistant.",
      img: ""
    },
    {
      label: "Privacy-Invariant",
      desc: "On-device processing wherever possible, encrypted local message vaults, minimal server knowledge by design, TTL-bound telemetry, no raw text or media retained server-side. Privacy isn't a feature—it's the foundation.",
      img: ""
    },
    {
      label: "Campus-First",
      desc: "Starting with college campuses where density, proximity, and trust matter most. Reaching privacy-conscious students through campus ambassadors, overcoming safety fears with offline-capable, mutual-reveal architecture.",
      img: ""
    },
    {
      label: "No Dark Patterns",
      desc: "No feeds, no infinite scroll, no 'who liked you' mechanics, no blurred photos as leverage, no manufactured scarcity. Rejects anxiety-based monetization and any mechanic that degrades user dignity, regardless of revenue upside.",
      img: ""
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      What makes Seven Degrees different? Here's what we stand for and how we're building the future of proximity networking.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/2">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
      </div>
    {/each}
  </div>
</section>
