<script setup lang="ts">
import { ref } from "vue";

const open = ref(false);
</script>

<template>
  <header class="absolute top-0 left-0 right-0 z-20 bg-red-100 px-8 py-6 md:px-32 md:py-9">

    <div class="flex justify-between items-center">
      <img src="/images/logo-dark.svg" alt="Logo" />

      <nav class="hidden md:flex justify-between items-center w-[65%]">
        <ul class="flex space-x-10">
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Contact</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">Careers</a></li>
        </ul>
        <a href="#" class="bg-emerald-300 py-2 px-8 rounded-4xl">Request Invite</a>
      </nav>

      <button class="md:hidden" @click="open = !open">
        <img v-if="!open" src="/images/icon-hamburger.svg" alt="Menu" />
        <img v-else src="/images/icon-close.svg" alt="Close" />
      </button>
    </div>

    <div
        x-show="open"
        :class="open ? 'max-h-96 opacity-100 scale-y-100' : 'max-h-0 opacity-0 scale-y-0'"
        class="md:hidden overflow-hidden transition-all duration-300 origin-top bg-white rounded-lg shadow-lg mt-4 p-6"
    >
      <ul class="flex flex-col space-y-6 text-center">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
        <li><a href="#">Blog</a></li>
        <li><a href="#">Careers</a></li>
      </ul>

      <div class="text-center mt-6">
        <a href="#" class="bg-emerald-300 py-2 px-8 rounded-4xl inline-block">
          Request Invite
        </a>
      </div>
    </div>

  </header>
</template>
