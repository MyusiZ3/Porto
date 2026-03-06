<template>
  <nav
    class="bg-[#171717] backdrop-blur-md py-2 px-19 sticky top-0 z-50 transition-all duration-300"
  >
    <div
      class="container mx-auto flex justify-between items-center gap-2 px-6 lg:px-18"
    >
      <div class="flex items-center gap-2">
        <img src="/images/logo.png" alt="logo" class="w-12 lg:w-14" />
        <a
          href="#"
          class="text-white font-semibold text-[13px] lg:text-[15px] font-['Poppins']"
          >Muhamad<br />Sidik</a
        >
      </div>
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
      <button
        class="lg:hidden text-white text-3xl hover:text-violet-500 transition"
      >
        <i class="bi bi-list"></i>
      </button>
    </div>
  </nav>
</template>
