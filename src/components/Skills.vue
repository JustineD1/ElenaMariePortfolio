<!-- components/Skills.vue -->
<script setup>
const skills = [
  'Administrative Support', 'Email Management', 'Calendar & Schedule Management',
  'Online Research', 'File Organization (Google Drive / MS Office)', 'Customer Service Support',
  'Phone, Chat, and Email Handling', 'Microsoft Office (Word, Excel, PowerPoint)',
  'Online Instruction & Tutoring', 'Strong Work Ethic'
] //[cite: 12]
</script>

<template>
  <section class="py-16 md:py-24 border-t border-emerald-100/50">
    <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 md:gap-12">
      
      <!-- Section Label -->
      <div class="lg:col-span-4">
        <div class="sticky top-24 space-y-2">
          <h2 class="text-3xl md:text-4xl font-black text-slate-950 tracking-tight">
            Skills & Modules
          </h2>
          <div class="h-1 w-12 bg-emerald-500 rounded-full mt-4"></div>
        </div>
      </div>

      <!-- Skills Area[cite: 12] -->
      <div class="lg:col-span-8">
        <div class="flex flex-wrap gap-3">
          <span 
            v-for="skill in skills" 
            :key="skill" 
            class="border border-slate-200/60 hover:border-emerald-500/80 text-slate-700 hover:text-emerald-700 hover:bg-emerald-50/40 hover:-translate-y-0.5 px-6 py-3 rounded-full text-xs font-semibold tracking-wide transition-all duration-300 bg-white cursor-default shadow-sm hover:shadow-md"
          >
            <!-- Sleek interactive leading dot -->
            <span class="inline-block h-1.5 w-1.5 rounded-full bg-emerald-500/40 group-hover:bg-emerald-500 mr-2"></span>
            {{ skill }}
          </span>
        </div>
      </div>

    </div>
  </section>
</template>