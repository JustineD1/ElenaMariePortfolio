<!-- components/Education.vue -->
<template>
  <section class="py-16 md:py-24 border-t border-emerald-100/50">
    <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 md:gap-12">
      
      <!-- Section Label -->
      <div class="lg:col-span-4">
        <div class="sticky top-24 space-y-2">
          <h2 class="text-3xl md:text-4xl font-black text-slate-950 tracking-tight">
            Education
          </h2>
          <div class="h-1 w-12 bg-emerald-500 rounded-full mt-4"></div>
        </div>
      </div>

      <!-- Education Grid[cite: 9] -->
      <div class="lg:col-span-8 grid grid-cols-1 md:grid-cols-2 gap-6">
        
        <!-- College[cite: 9] -->
        <div class="bg-white/50 border border-emerald-100/50 hover:border-emerald-500/50 p-6 rounded-2xl shadow-sm hover:shadow-md transition-all duration-300 flex flex-col justify-between">
          <div class="space-y-3">
            <span class="text-[9px] font-mono font-bold text-emerald-600 tracking-widest uppercase px-2.5 py-1 bg-emerald-50 rounded-full">HIGHER EDUCATION</span>
            <h3 class="font-extrabold text-slate-950 text-xl tracking-tight">Davao del Norte State College</h3>
            <p class="text-sm text-slate-500">Bachelor of Arts in Communication</p>
          </div>
          <div class="mt-6 pt-4 border-t border-slate-100 flex items-center justify-between">
            <span class="text-xs font-mono font-extrabold text-emerald-600">2021 - 2025</span>
            <span class="h-1.5 w-1.5 rounded-full bg-emerald-500"></span>
          </div>
        </div>
        
        <!-- Senior High[cite: 9] -->
        <div class="bg-white/50 border border-slate-100 p-6 rounded-2xl shadow-sm hover:shadow-md transition-all duration-300 flex flex-col justify-between">
          <div class="space-y-3">
            <span class="text-[9px] font-mono font-bold text-slate-400 tracking-widest uppercase px-2.5 py-1 bg-slate-50 rounded-full">SENIOR HIGH SCHOOL</span>
            <h3 class="font-extrabold text-slate-950 text-xl tracking-tight">Panabo City Senior High School</h3>
            <p class="text-sm text-slate-500">Humanities and Social Sciences</p>
          </div>
          <div class="mt-6 pt-4 border-t border-slate-100 flex items-center justify-between">
            <span class="text-xs font-mono font-bold text-slate-500">2019 - 2021</span>
            <span class="h-1.5 w-1.5 rounded-full bg-slate-300"></span>
          </div>
        </div>

        <!-- Junior High[cite: 9] -->
        <div class="bg-white/50 border border-slate-100 p-6 rounded-2xl shadow-sm hover:shadow-md transition-all duration-300 flex flex-col justify-between">
          <div class="space-y-3">
            <span class="text-[9px] font-mono font-bold text-slate-400 tracking-widest uppercase px-2.5 py-1 bg-slate-50 rounded-full">SECONDARY EDUCATION</span>
            <h3 class="font-extrabold text-slate-950 text-xl tracking-tight">Panabo National High School</h3>
            <p class="text-sm text-slate-500">Secondary Education</p>
          </div>
          <div class="mt-6 pt-4 border-t border-slate-100 flex items-center justify-between">
            <span class="text-xs font-mono font-bold text-slate-500">2015 - 2019</span>
            <span class="h-1.5 w-1.5 rounded-full bg-slate-300"></span>
          </div>
        </div>

        <!-- Elementary[cite: 9] -->
        <div class="bg-white/50 border border-slate-100 p-6 rounded-2xl shadow-sm hover:shadow-md transition-all duration-300 flex flex-col justify-between">
          <div class="space-y-3">
            <span class="text-[9px] font-mono font-bold text-slate-400 tracking-widest uppercase px-2.5 py-1 bg-slate-50 rounded-full">PRIMARY EDUCATION</span>
            <h3 class="font-extrabold text-slate-950 text-xl tracking-tight">Panabo Central Elementary School</h3>
            <p class="text-sm text-slate-500">Elementary Education</p>
          </div>
          <div class="mt-6 pt-4 border-t border-slate-100 flex items-center justify-between">
            <span class="text-xs font-mono font-bold text-slate-500">2009 - 2015</span>
            <span class="h-1.5 w-1.5 rounded-full bg-slate-300"></span>
          </div>
        </div>

      </div>

    </div>
  </section>
</template>