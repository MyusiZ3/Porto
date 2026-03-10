<script setup>
import { ref } from 'vue';

const isMenuOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};
</script>

<template>
  <nav
    class="bg-[#171717]/100 backdrop-blur-md py-3 lg:py-3 sticky top-0 z-50 transition-all duration-300"
  >
    <div
      class="container mx-auto flex justify-between items-center gap-2 px-6 lg:px-38"
    >
      <div class="flex items-center gap-2 relative z-50">
        <img src="/images/logo.png" alt="logo" class="w-10 lg:w-14" />
        <a
          href="#"
          class="text-white font-semibold text-[13px] lg:text-[15px] font-['Poppins']"
          >Muhamad<br />Sidik</a
        >
      </div>
      
      <!-- Desktop Menu -->
      <div class="hidden lg:flex items-center gap-14 uppercase">
        <a
          href="#"
          class="text-white font-bold text-[13px] lg:text-[15px] font-['Roboto'] hover:text-violet-500 transition"
          >Home</a
        >
        <a
          href="#about"
          class="text-white font-bold text-[13px] lg:text-[15px] font-['Roboto'] hover:text-violet-500 transition"
          >About</a
        >
        <a
          href="#experience"
          class="text-white font-bold text-[13px] lg:text-[15px] font-['Roboto'] hover:text-violet-500 transition"
          >Experience</a
        >
        <a
          href="#skills"
          class="text-white font-bold text-[13px] lg:text-[15px] font-['Roboto'] hover:text-violet-500 transition"
          >Skills</a
        >
        <a
          href="#experience"
          class="text-white font-bold text-[13px] lg:text-[15px] font-['Roboto'] hover:text-violet-500 transition"
          >Work</a
        >
        <a
          href="#contact"
          class="text-white font-bold text-[13px] lg:text-[15px] font-['Roboto'] hover:text-violet-500 transition"
          >Contact Me</a
        >
        <button
          class="w-8 h-8 flex items-center justify-center bg-violet-500 text-white rounded-[10px] hover:bg-violet-600 transition font-bold text-[13px] lg:text-[15px] font-['Roboto']"
        >
          ID
        </button>
      </div>

      <!-- Mobile Hamburger Button -->
      <button
        @click="toggleMenu"
        class="lg:hidden text-white text-3xl hover:text-violet-500 transition relative z-50"
      >
        <i :class="isMenuOpen ? 'bi bi-x' : 'bi bi-list'"></i>
      </button>
    </div>

    <!-- Mobile Menu Overlay -->
    <div
      class="lg:hidden fixed inset-x-0 top-[60px] bg-[#171717]/95 backdrop-blur-md border-t border-gray-800 transition-all duration-300 ease-in-out shadow-2xl z-40"
      :class="isMenuOpen ? 'max-h-screen py-6 opacity-100 visible' : 'max-h-0 py-0 opacity-0 invisible'"
    >
      <div class="flex flex-col items-center gap-6 uppercase overflow-hidden">
        <a
          href="#"
          @click="isMenuOpen = false"
          class="text-white font-bold text-[14px] font-['Roboto'] hover:text-violet-500 transition"
          >Home</a
        >
        <a
          href="#about"
          @click="isMenuOpen = false"
          class="text-white font-bold text-[14px] font-['Roboto'] hover:text-violet-500 transition"
          >About</a
        >
        <a
          href="#experience"
          @click="isMenuOpen = false"
          class="text-white font-bold text-[14px] font-['Roboto'] hover:text-violet-500 transition"
          >Experience</a
        >
        <a
          href="#skills"
          @click="isMenuOpen = false"
          class="text-white font-bold text-[14px] font-['Roboto'] hover:text-violet-500 transition"
          >Skills</a
        >
        <a
          href="#experience"
          @click="isMenuOpen = false"
          class="text-white font-bold text-[14px] font-['Roboto'] hover:text-violet-500 transition"
          >Work</a
        >
        <a
          href="#contact"
          @click="isMenuOpen = false"
          class="text-white font-bold text-[14px] font-['Roboto'] hover:text-violet-500 transition"
          >Contact Me</a
        >
        <button
          @click="isMenuOpen = false"
          class="w-10 h-10 flex items-center justify-center bg-violet-500 text-white rounded-[10px] hover:bg-violet-600 transition font-bold text-[14px] font-['Roboto'] mt-2"
        >
          ID
        </button>
      </div>
    </div>
  </nav>
</template>
