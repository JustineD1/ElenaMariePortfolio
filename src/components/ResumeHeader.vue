<!-- src/components/ResumeHeader.vue -->
<template>
  <header class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center py-8 md:py-16">
    
    <!-- Hero Text & CTA -->
    <div class="lg:col-span-7 space-y-6 text-left">
      <div class="space-y-4">
        <h1 class="text-6xl sm:text-7xl md:text-8xl lg:text-[5.5rem] xl:text-[6.5rem] font-black tracking-tight text-slate-950 leading-[1.05]">
          Hi, I'm Elena
        </h1>
        <p class="text-2xl md:text-3xl lg:text-4xl font-extrabold text-emerald-600 tracking-wide">
          Communication Specialist / Professional Instructor
        </p>
      </div>

      <!-- Main description -->
      <p class="text-slate-600 text-base md:text-lg leading-relaxed max-w-2xl font-light">
        A passionate Bachelor of Arts in Communication graduate with professional experience bridging client success, online instruction, and public service. I specialize in crafting seamless interpersonal connections and delivering responsive support.
      </p>

      <!-- Action Buttons -->
      <div class="flex flex-wrap gap-4 pt-4">
        <!-- About Me Button -->
        <a href="#about" class="border border-slate-200 hover:border-slate-300 hover:bg-slate-50 text-slate-700 rounded-full transition-all duration-300 px-10 py-4 text-xs font-bold tracking-widest uppercase">
          About Me
        </a>
        
        <!-- Direct Gmail Contact Button -->
        <a 
          href="https://mail.google.com/mail/?view=cm&fs=1&to=Mynameiselena123@gmail.com" 
          target="_blank" 
          rel="noopener noreferrer"
          class="bg-emerald-600 hover:bg-emerald-700 text-white rounded-full transition-all duration-300 px-10 py-4 text-xs font-bold tracking-widest uppercase shadow-md shadow-emerald-600/10"
        >
          Contact Me
        </a>
      </div>
    </div>
    
    <!-- Portrait Side -->
    <div class="lg:col-span-5 flex justify-center lg:justify-end relative">
      <div class="absolute inset-0 bg-gradient-to-tr from-emerald-100 to-transparent rounded-full blur-3xl pointer-events-none"></div>
      
      <div class="relative w-72 h-72 md:w-96 md:h-96 overflow-hidden rounded-3xl group">
        <img 
          src="../assets/pic.png" 
          alt="Elena" 
          class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" 
        />
        <div class="absolute inset-0 bg-gradient-to-t from-[#fbfdfc] via-transparent to-transparent opacity-80"></div>
      </div>
    </div>

  </header>
</template>