<!-- components/Experience.vue -->
<template>
  <section class="py-16 md:py-24 border-t border-emerald-100/50">
    <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 md:gap-12">
      
      <!-- Section Label -->
      <div class="lg:col-span-4">
        <div class="sticky top-24 space-y-2">
          <h2 class="text-3xl md:text-4xl font-black text-slate-950 tracking-tight">
            Professional Experience
          </h2>
          <div class="h-1 w-12 bg-emerald-500 rounded-full mt-4"></div>
        </div>
      </div>

      <!-- Experience Stream[cite: 10] -->
      <div class="lg:col-span-8 space-y-8">
        
        <!-- Experience Item 1[cite: 10] -->
        <div class="group relative pl-8 pb-4 border-l border-slate-200/80 hover:border-emerald-500 transition-colors duration-500">
          <!-- Active Marker Dot -->
          <div class="absolute -left-[5px] top-2.5 h-2.5 w-2.5 rounded-full bg-slate-300 group-hover:bg-emerald-500 group-hover:scale-150 group-hover:ring-4 group-hover:ring-emerald-100 transition-all duration-500"></div>
          
          <div class="bg-white/50 border border-slate-100/60 rounded-2xl p-6 shadow-sm hover:shadow-md hover:bg-white transition-all duration-500 space-y-3">
            <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2">
              <h3 class="font-bold text-slate-950 text-xl group-hover:text-emerald-600 transition-colors">
                Local Government Unit Employee
              </h3>
              <span class="inline-block px-3 py-1 bg-emerald-50 text-emerald-700 text-xs font-mono font-bold rounded-full self-start sm:self-auto shadow-sm shadow-emerald-600/5">
                2025 - 2026
              </span>
            </div>
            
            <div class="flex items-center gap-2 text-xs font-semibold text-slate-400 tracking-wider uppercase">
              <span>City Government of Panabo</span>
              <span>•</span>
              <span class="text-emerald-600">Administrative Support</span>
            </div>
            
            <p class="text-sm text-slate-500 font-light leading-relaxed">
              A local government staff member involved in administrative work, public service delivery, and support in implementing government programs and community services.
            </p>
          </div>
        </div>

        <!-- Experience Item 2[cite: 10] -->
        <div class="group relative pl-8 pb-4 border-l border-slate-200/80 hover:border-emerald-500 transition-colors duration-500">
          <div class="absolute -left-[5px] top-2.5 h-2.5 w-2.5 rounded-full bg-slate-300 group-hover:bg-emerald-500 group-hover:scale-150 group-hover:ring-4 group-hover:ring-emerald-100 transition-all duration-500"></div>
          
          <div class="bg-white/50 border border-slate-100/60 rounded-2xl p-6 shadow-sm hover:shadow-md hover:bg-white transition-all duration-500 space-y-3">
            <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2">
              <h3 class="font-bold text-slate-950 text-xl group-hover:text-emerald-600 transition-colors">
                Call Center Agent
              </h3>
              <span class="inline-block px-3 py-1 bg-emerald-50 text-emerald-700 text-xs font-mono font-bold rounded-full self-start sm:self-auto shadow-sm shadow-emerald-600/5">
                2023 - 2025
              </span>
            </div>
            
            <div class="flex items-center gap-2 text-xs font-semibold text-slate-400 tracking-wider uppercase">
              <span>iQor - Davao</span>
              <span>•</span>
              <span class="text-emerald-600">Customer Success</span>
            </div>
            
            <p class="text-sm text-slate-500 font-light leading-relaxed">
              Handled inbound customer service calls, assisting with product inquiries, order issues, billing, and account troubleshooting.
            </p>
          </div>
        </div>

        <!-- Experience Item 3[cite: 10] -->
        <div class="group relative pl-8 border-l border-slate-200/80 hover:border-emerald-500 transition-colors duration-500">
          <div class="absolute -left-[5px] top-2.5 h-2.5 w-2.5 rounded-full bg-slate-300 group-hover:bg-emerald-500 group-hover:scale-150 group-hover:ring-4 group-hover:ring-emerald-100 transition-all duration-500"></div>
          
          <div class="bg-white/50 border border-slate-100/60 rounded-2xl p-6 shadow-sm hover:shadow-md hover:bg-white transition-all duration-500 space-y-3">
            <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2">
              <h3 class="font-bold text-slate-950 text-xl group-hover:text-emerald-600 transition-colors">
                English as a Second Language (ESL) Tutor
              </h3>
              <span class="inline-block px-3 py-1 bg-emerald-50 text-emerald-700 text-xs font-mono font-bold rounded-full self-start sm:self-auto shadow-sm shadow-emerald-600/5">
                2023
              </span>
            </div>
            
            <div class="flex items-center gap-2 text-xs font-semibold text-slate-400 tracking-wider uppercase">
              <span>Acadsoc</span>
              <span>•</span>
              <span class="text-emerald-600">Online Pedagogy</span>
            </div>
            
            <p class="text-sm text-slate-500 font-light leading-relaxed">
              Taught English to international students of different ages and levels through online classes.
            </p>
          </div>
        </div>

      </div>

    </div>
  </section>
</template>