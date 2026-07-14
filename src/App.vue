<!-- src/App.vue -->
<script setup>
import { ref, onMounted } from "vue";
import ResumeHeader from "./components/ResumeHeader.vue";
import AboutMe from "./components/AboutMe.vue";
import Experience from "./components/Experience.vue";
import Education from "./components/Education.vue";
import Skills from "./components/Skills.vue";
import PersonalBackground from "./components/PersonalBackground.vue";
import ContactFooter from "./components/ContactFooter.vue";
import Trainings from "./components/Trainings.vue"; // Added Import

const isMobileMenuOpen = ref(false);
const showIntro = ref(true);
const isLeaving = ref(false);

onMounted(() => {
  document.body.style.overflow = "hidden";

  setTimeout(() => {
    isLeaving.value = true;
  }, 2000);

  setTimeout(() => {
    showIntro.value = false;
    document.body.style.overflow = "";
  }, 3200);
});
</script>

<template>
  <!-- Architectural Shutter Intro Screen -->
  <div
    v-if="showIntro"
    class="fixed inset-0 z-[100] flex overflow-hidden pointer-events-none"
  >
    <div class="h-full w-1/3 bg-emerald-900 border-r border-emerald-800/20 transition-transform duration-[1000ms] ease-[cubic-bezier(0.85,0,0.15,1)] will-change-transform pointer-events-auto" :class="{ '-translate-y-full': isLeaving }"></div>
    <div class="h-full w-1/3 bg-emerald-900 border-r border-emerald-800/20 transition-transform duration-[1000ms] delay-150 ease-[cubic-bezier(0.85,0,0.15,1)] will-change-transform pointer-events-auto" :class="{ '-translate-y-full': isLeaving }"></div>
    <div class="h-full w-1/3 bg-emerald-900 transition-transform duration-[1000ms] delay-300 ease-[cubic-bezier(0.85,0,0.15,1)] will-change-transform pointer-events-auto" :class="{ '-translate-y-full': isLeaving }"></div>

    <div class="absolute inset-0 flex flex-col items-center justify-center text-center transition-all duration-500 ease-out" :class="{ 'opacity-0 scale-90 blur-sm pointer-events-none': isLeaving }">
      <div class="space-y-6 px-6 relative">
        <div class="inline-flex items-center gap-2 border border-white/20 bg-white/10 px-4 py-1.5 rounded-full backdrop-blur-sm">
          <span class="h-1.5 w-1.5 rounded-full bg-white animate-ping"></span>
          <span class="text-[9px] font-mono font-bold tracking-[0.25em] text-emerald-200 uppercase pl-[0.25em]">Online Portfolio</span>
        </div>
        <div class="space-y-1">
          <h1 class="text-4xl md:text-5xl font-black tracking-tight text-white uppercase">ELENA<span class="text-emerald-300">_</span>M</h1>
          <p class="text-[11px] font-mono text-emerald-100/60 tracking-[0.4em] uppercase pl-[0.4em]">Curated Showcase</p>
        </div>
        <div class="w-12 h-[1px] bg-white/20 mx-auto overflow-hidden relative">
          <div class="absolute inset-0 bg-gradient-to-r from-transparent via-white to-transparent animate-line-sweep"></div>
        </div>
      </div>
    </div>
  </div>

  <div class="min-h-screen bg-[#fbfdfc] text-slate-600 font-sans antialiased selection:bg-emerald-100 selection:text-emerald-800 relative overflow-x-hidden">
    <div class="absolute top-0 right-0 w-[800px] h-[600px] bg-emerald-100/30 rounded-full blur-[160px] pointer-events-none"></div>
    <div class="absolute top-1/3 left-0 w-[600px] h-[600px] bg-emerald-50/40 rounded-full blur-[140px] pointer-events-none"></div>

    <nav class="sticky top-0 z-50 bg-[#fbfdfc]/80 backdrop-blur-lg border-b border-emerald-100/40">
      <div class="max-w-5xl mx-auto px-6 sm:px-8">
        <div class="flex items-center justify-between h-20">
          <div class="flex-shrink-0">
            <a href="#" class="flex items-center gap-2 text-sm font-bold tracking-widest text-slate-900 uppercase">
              <img src="/src/assets/pic2.png" alt="Logo" class="h-8 w-auto" />
              My Portfolio
            </a>
          </div>

          <div class="hidden md:block">
            <div class="ml-10 flex items-baseline space-x-8 text-[11px] font-semibold tracking-widest text-slate-500 uppercase">
              <a href="#about" class="hover:text-emerald-600 transition-colors">About</a>
              <a href="#experience" class="hover:text-emerald-600 transition-colors">Experience</a>
              <a href="#education" class="hover:text-emerald-600 transition-colors">Education</a>
              <a href="#skills" class="hover:text-emerald-600 transition-colors">Skills</a>
              <a href="#personal" class="hover:text-emerald-600 transition-colors">Profile</a>
              <a href="#trainings" class="hover:text-emerald-600 transition-colors">Trainings</a> <!-- Added Link -->
              <a href="#contact" class="hover:text-emerald-600 transition-colors">Contact</a>
            </div>
          </div>

          <div class="md:hidden">
            <button @click="isMobileMenuOpen = !isMobileMenuOpen" type="button" class="text-slate-500 hover:text-emerald-600 p-2 focus:outline-none transition-colors">
              <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path v-if="!isMobileMenuOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M4 6h16M4 12h16M4 18h16" />
                <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M6 18L18 6M6 6l12 12" />
              </svg>
            </button>
          </div>
        </div>
      </div>

      <div v-show="isMobileMenuOpen" class="md:hidden bg-[#fbfdfc] border-b border-emerald-100/40 py-4">
        <div class="px-6 space-y-4 text-[11px] font-semibold tracking-widest text-slate-500 uppercase">
          <a href="#about" @click="isMobileMenuOpen = false" class="block hover:text-emerald-600">About</a>
          <a href="#experience" @click="isMobileMenuOpen = false" class="block hover:text-emerald-600">Experience</a>
          <a href="#education" @click="isMobileMenuOpen = false" class="block hover:text-emerald-600">Education</a>
          <a href="#skills" @click="isMobileMenuOpen = false" class="block hover:text-emerald-600">Skills</a>
          <a href="#personal" @click="isMobileMenuOpen = false" class="block hover:text-emerald-600">Profile</a>
          <a href="#trainings" @click="isMobileMenuOpen = false" class="block hover:text-emerald-600">Trainings</a> <!-- Added Link -->
          <a href="#contact" @click="isMobileMenuOpen = false" class="block hover:text-emerald-600">Contact</a>
        </div>
      </div>
    </nav>

    <main v-if="!showIntro || isLeaving" class="max-w-5xl mx-auto px-6 sm:px-8 space-y-8 relative z-10">
      <div class="animate-reveal"><ResumeHeader /></div>
      <div id="about" class="animate-reveal scroll-mt-24"><AboutMe /></div>
      <div id="experience" class="animate-reveal scroll-mt-24"><Experience /></div>
      <div id="education" class="animate-reveal scroll-mt-24"><Education /></div>
      <div id="trainings" class="animate-reveal scroll-mt-24"><Trainings /></div> <!-- Added Component -->
      <div id="skills" class="animate-reveal scroll-mt-24"><Skills /></div>
      <div id="personal" class="animate-reveal scroll-mt-24"><PersonalBackground /></div>
    </main>

    <ContactFooter v-if="!showIntro || isLeaving" />
  </div>
</template>

<style>
html { scroll-behavior: smooth; }
@keyframes accentSweep { 0% { transform: translateX(-100%); } 50%, 100% { transform: translateX(100%); } }
.animate-line-sweep { animation: accentSweep 2.5s ease-in-out infinite; }
@keyframes contentReveal { from { opacity: 0; transform: translateY(24px); } to { opacity: 1; transform: translateY(0); } }
.animate-reveal { animation: contentReveal 1.2s cubic-bezier(0.16, 1, 0.3, 1) both; }
.animate-reveal:nth-child(1) { animation-delay: 150ms; }
.animate-reveal:nth-child(2) { animation-delay: 250ms; }
.animate-reveal:nth-child(3) { animation-delay: 350ms; }
.animate-reveal:nth-child(4) { animation-delay: 450ms; }
.animate-reveal:nth-child(5) { animation-delay: 550ms; }
.animate-reveal:nth-child(6) { animation-delay: 650ms; }
.animate-reveal:nth-child(7) { animation-delay: 750ms; } /* Added animation delay for new section */
</style>