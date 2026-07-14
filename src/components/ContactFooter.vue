<!-- components/ContactFooter.vue -->
<template>
  <footer id="contact" class="mt-24 border-t border-emerald-100/50 bg-gradient-to-b from-transparent to-[#f4f8f6]/40 relative overflow-hidden">
    <!-- Ambient background glow behind footer -->
    <div class="absolute bottom-0 right-1/4 w-[500px] h-[300px] bg-emerald-100/20 rounded-full blur-[120px] pointer-events-none"></div>

    <div class="max-w-5xl mx-auto px-6 sm:px-8 py-16 md:py-24 relative z-10">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
        
        <!-- Let's Connect Copy -->
        <div class="lg:col-span-7 space-y-6">
          <span class="text-[10px] font-mono font-bold text-emerald-600 tracking-widest uppercase">GET IN TOUCH</span>
          <h2 class="text-4xl md:text-5xl font-black text-slate-950 tracking-tight leading-none">
            Let's work together.
          </h2>
          <p class="text-slate-500 text-base md:text-lg font-light leading-relaxed max-w-lg">
            Whether you're looking for administrative support, a professional communication specialist, or an engaging online instructor, I'd love to connect and discuss how I can help your team.
          </p>
          <div class="pt-2">
            <!-- Direct Gmail Compose Button -->
            <a 
              href="https://mail.google.com/mail/?view=cm&fs=1&to=Mynameiselena123@gmail.com" 
              target="_blank"
              rel="noopener noreferrer"
              class="inline-flex items-center gap-3 bg-emerald-600 hover:bg-emerald-700 text-white rounded-full transition-all duration-300 px-8 py-4 text-xs font-bold tracking-widest uppercase shadow-md shadow-emerald-600/10"
            >
              <span>Send an Email</span>
              <svg class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M14 5l7 7m0 0l-7 7m7-7H3" />
              </svg>
            </a>
          </div>
        </div>

        <!-- Contact Box Info -->
        <div class="lg:col-span-5 bg-white border border-slate-100 rounded-3xl p-8 shadow-sm space-y-6">
          <h3 class="text-xs font-bold text-slate-400 uppercase tracking-widest font-mono">Contact Details</h3>
          
          <div class="space-y-4">
            <!-- Email Info -->
            <div class="flex items-start gap-4">
              <div class="p-2 bg-emerald-50 rounded-xl text-emerald-600">
                <svg class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                </svg>
              </div>
              <div>
                <p class="text-[10px] text-slate-400 uppercase tracking-widest font-mono">Email Me Directly</p>
                <!-- Direct Gmail Text Link -->
                <a 
                  href="https://mail.google.com/mail/?view=cm&fs=1&to=Mynameiselena123@gmail.com" 
                  target="_blank"
                  rel="noopener noreferrer"
                  class="text-sm font-semibold text-slate-800 hover:text-emerald-600 transition-colors break-all"
                >
                  Mynameiselena123@gmail.com
                </a>
              </div>
            </div>

            <!-- Location Info -->
            <div class="flex items-start gap-4">
              <div class="p-2 bg-emerald-50 rounded-xl text-emerald-600">
                <svg class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                  <path stroke-linecap="round" stroke-linejoin="round" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                </svg>
              </div>
              <div>
                <p class="text-[10px] text-slate-400 uppercase tracking-widest font-mono">Location</p>
                <p class="text-sm font-semibold text-slate-800">
                  City of Davao, Davao del Sur, Philippines
                </p>
              </div>
            </div>
          </div>
        </div>

      </div>

      <!-- Bottom copyright and quick links -->
      <div class="mt-20 pt-8 border-t border-slate-200/60 flex flex-col md:flex-row items-center justify-between gap-4 text-xs font-medium text-slate-400">
        <p>© 2026 Elena. All rights reserved.</p>
        <div class="flex gap-6 uppercase tracking-wider font-semibold text-[10px]">
          <a href="#about" class="hover:text-emerald-600 transition-colors">About</a>
          <a href="#experience" class="hover:text-emerald-600 transition-colors">Experience</a>
          <a href="#education" class="hover:text-emerald-600 transition-colors">Education</a>
          <a href="#skills" class="hover:text-emerald-600 transition-colors">Skills</a>
          <a href="#personal" class="hover:text-emerald-600 transition-colors">Profile</a>
        </div>
      </div>
    </div>
  </footer>
</template>