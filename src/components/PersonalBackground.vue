<!-- components/PersonalBackground.vue -->
<template>
  <section class="py-16 md:py-24 border-t border-emerald-100/50">
    <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 md:gap-12">
      
      <!-- Section Label -->
      <div class="lg:col-span-4">
        <div class="sticky top-24 space-y-2">
          <h2 class="text-3xl md:text-4xl font-black text-slate-950 tracking-tight">
            Personal Data
          </h2>
          <div class="h-1 w-12 bg-emerald-500 rounded-full mt-4"></div>
        </div>
      </div>

      <!-- Personal Info Grid[cite: 11] -->
      <div class="lg:col-span-8 bg-white/40 border border-slate-100 rounded-2xl p-8 shadow-sm">
        <div class="grid grid-cols-2 md:grid-cols-3 gap-8">
          
          <!-- DOB[cite: 11] -->
          <div class="space-y-1">
            <p class="text-[10px] text-slate-400 uppercase tracking-widest font-mono font-bold">Date of Birth</p>
            <p class="font-bold text-slate-900 text-sm md:text-base">September 15, 2002</p>
          </div>

          <!-- POB[cite: 11] -->
          <div class="space-y-1">
            <p class="text-[10px] text-slate-400 uppercase tracking-widest font-mono font-bold">Place of Birth</p>
            <p class="font-bold text-slate-900 text-sm md:text-base">City of Davao, Davao del Sur</p>
          </div>

          <!-- Civil Status[cite: 11] -->
          <div class="space-y-1">
            <p class="text-[10px] text-slate-400 uppercase tracking-widest font-mono font-bold">Civil Status</p>
            <p class="font-bold text-slate-900 text-sm md:text-base">Single</p>
          </div>

          <!-- Age[cite: 11] -->
          <div class="space-y-1">
            <p class="text-[10px] text-slate-400 uppercase tracking-widest font-mono font-bold">Age</p>
            <p class="font-bold text-slate-900 text-sm md:text-base">23</p>
          </div>

          <!-- Height[cite: 11] -->
          <div class="space-y-1">
            <p class="text-[10px] text-slate-400 uppercase tracking-widest font-mono font-bold">Height</p>
            <p class="font-bold text-slate-900 text-sm md:text-base">1.49m</p>
          </div>

          <!-- Weight[cite: 11] -->
          <div class="space-y-1">
            <p class="text-[10px] text-slate-400 uppercase tracking-widest font-mono font-bold">Weight</p>
            <p class="font-bold text-slate-900 text-sm md:text-base">46kg</p>
          </div>

        </div>
      </div>

    </div>
  </section>
</template>