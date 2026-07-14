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
import Trainings from "./components/Trainings.vue";

const isMobileMenuOpen = ref(false);
const showIntro = ref(true);
const isLeaving = ref(false);

onMounted(() => {
  document.body.style.overflow = "hidden";
  setTimeout(() => { isLeaving.value = true; }, 2000);
  setTimeout(() => { showIntro.value = false; document.body.style.overflow = ""; }, 3200);
});
</script>

<template>
  <!-- Architectural Shutter Intro Screen -->
  <div v-if="showIntro" class="fixed inset-0 z-[100] flex overflow-hidden pointer-events-none">
    <div class="h-full w-1/3 bg-emerald-900 border-r border-emerald-800/20 transition-transform duration-[1000ms] ease-[cubic-bezier(0.85,0,0.15,1)] will-change-transform pointer-events-auto" :class="{ '-translate-y-full': isLeaving }"></div>
    <div class="h-full w-1/3 bg-emerald-900 border-r border-emerald-800/20 transition-transform duration-[1000ms] delay-150 ease-[cubic-bezier(0.85,0,0.15,1)] will-change-transform pointer-events-auto" :class="{ '-translate-y-full': isLeaving }"></div>
    <div class="h-full w-1/3 bg-emerald-900 transition-transform duration-[1000ms] delay-300 ease-[cubic-bezier(0.85,0,0.15,1)] will-change-transform pointer-events-auto" :class="{ '-translate-y-full': isLeaving }"></div>
  </div>

  <div class="min-h-screen bg-[#fbfdfc] text-slate-600 font-sans antialiased relative overflow-x-hidden">
    <!-- Navigation -->
    <nav class="sticky top-0 z-50 bg-[#fbfdfc]/80 backdrop-blur-lg border-b border-emerald-100/40">
      <div class="max-w-5xl mx-auto px-6 sm:px-8">
        <div class="flex items-center justify-between h-20">
          <a href="#" class="flex items-center gap-2 text-sm font-bold tracking-widest text-slate-900 uppercase">
             My Portfolio
          </a>
          <!-- Menu Items -->
          <div class="hidden md:flex ml-10 space-x-8 text-[11px] font-semibold text-slate-500 uppercase">
              <a href="#about">About</a>
              <a href="#experience">Experience</a>
              <a href="#education">Education</a>
              <a href="#trainings">Trainings</a>
              <a href="#skills">Skills</a>
              <a href="#personal">Profile</a>
              <a href="#contact">Contact</a>
          </div>
        </div>
      </div>
    </nav>

    <!-- Main Content -->
    <main v-if="!showIntro || isLeaving" class="max-w-5xl mx-auto px-6 sm:px-8 space-y-8 relative z-10">
      <div class="animate-reveal"><ResumeHeader /></div>
      <div id="about" class="animate-reveal"><AboutMe /></div>
      <div id="experience" class="animate-reveal"><Experience /></div>
      <div id="education" class="animate-reveal"><Education /></div>
      <div id="trainings" class="animate-reveal"><Trainings /></div>
      <div id="skills" class="animate-reveal"><Skills /></div>
      <div id="personal" class="animate-reveal"><PersonalBackground /></div>
    </main>

    <!-- Centered Footer Fix -->
    <div v-if="!showIntro || isLeaving" class="max-w-5xl mx-auto px-6 sm:px-8 pb-12">
      <div id="contact" class="scroll-mt-24">
        <ContactFooter />
      </div>
    </div>
  </div>
</template>

<style>
/* Add your existing styles here */
html { scroll-behavior: smooth; }
.animate-reveal { animation: contentReveal 1.2s cubic-bezier(0.16, 1, 0.3, 1) both; }
@keyframes contentReveal { from { opacity: 0; transform: translateY(24px); } to { opacity: 1; transform: translateY(0); } }
</style>