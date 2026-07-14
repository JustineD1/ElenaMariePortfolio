<script setup>
const trainingEvents = [
  {
    date: "July 07, 2026",
    title: "MSME Success Talks",
    description: "Cafe Owners: Lessons, Leadership, and Customer-Centered Growth",
  },
  {
    date: "July 07, 2026",
    title: "Sweet Success",
    description: "Baking as a Business Opportunity",
  },
  {
    date: "July 08, 2026",
    title: "Business Continuity & Financial Literacy",
    description: "Strategic planning and financial management training.",
  },
  {
    date: "July 09, 2026",
    title: "Upskill to Upscale",
    description: "AI, Digital Marketing, E-commerce, Social Media Management, and Online Presence Workshop.",
  },
  {
    date: "July 10, 2026",
    title: "Basic Bookkeeping",
    description: "Essential training for MSME financial record keeping.",
  },
];
</script>

<template>
  <section id="trainings" class="py-12">
    <div class="mb-10">
      <h2 class="text-3xl font-black text-slate-900 tracking-tight">Trainings</h2>
      <p class="text-slate-500 mt-2">Professional development and workshops attended.</p>
    </div>

    <!-- Bento Grid Layout -->
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
      <div
        v-for="(event, index) in trainingEvents"
        :key="index"
        :class="[
          'relative p-6 rounded-3xl border border-slate-200 bg-white shadow-sm transition-all duration-300 hover:shadow-lg hover:-translate-y-1',
          index === 0 ? 'lg:col-span-2' : ''
        ]"
      >
        <div class="flex flex-col h-full justify-between">
          <div>
            <div class="flex items-center gap-2 mb-4">
              <span class="px-3 py-1 bg-emerald-100 text-emerald-700 text-[10px] font-bold uppercase tracking-wider rounded-full">
                MSME Week
              </span>
            </div>
            <h3 class="text-lg font-bold text-slate-900 mb-2 leading-tight">
              {{ event.title }}
            </h3>
            <p class="text-sm text-slate-500 leading-relaxed">
              {{ event.description }}
            </p>
          </div>
          
          <div class="mt-6 flex items-center justify-between">
            <span class="text-[11px] font-mono font-medium text-slate-400">
              {{ event.date }}
            </span>
            <div class="h-8 w-8 rounded-full bg-slate-50 flex items-center justify-center text-slate-300 group-hover:text-emerald-500 transition-colors">
              <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"/></svg>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>