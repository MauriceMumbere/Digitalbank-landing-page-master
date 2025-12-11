<script setup lang="ts">
import {ref} from "vue";

const open = ref(false);
</script>

<template>
  <header class="absolute top-0 left-0 right-0 z-20 bg-white px-8 py-6 md:px-32 md:py-7">

    <div class="flex justify-between items-center">
      <img src="/images/logo-dark.svg" alt="Logo"/>

      <nav class="hidden md:flex justify-between items-center w-[65%]">
        <ul class="flex space-x-10">
          <li>
            <a href="#"
               class="relative pb-1
            before:content-[''] before:absolute
            before:left-0 before:top-[60px]
            before:w-0 before:h-[3px]
            before:bg-green-500 before:transition-all before:duration-300
            hover:before:w-full text-gray-600">
              Home
            </a>
          </li>

          <li>
            <a href="#"
               class="relative pb-1
            before:content-[''] before:absolute
            before:left-0 before:top-[60px]
            before:w-0 before:h-[3px]
            before:bg-green-500 before:transition-all before:duration-300
            hover:before:w-full text-gray-600">
              About
            </a>
          </li>

          <li>
            <a href="#"
               class="relative pb-1
            before:content-[''] before:absolute
            before:left-0 before:top-[60px]
            before:w-0 before:h-[3px]
            before:bg-green-500 before:transition-all before:duration-300
            hover:before:w-full text-gray-600">
              Contact
            </a>
          </li>

          <li>
            <a href="#"
               class="relative pb-1
            before:content-[''] before:absolute
            before:left-0 before:top-[60px]
            before:w-0 before:h-[3px]
            before:bg-green-500 before:transition-all before:duration-300
            hover:before:w-full text-gray-600">
              Blog
            </a>
          </li>

          <li>
            <a href="#"
               class="relative pb-1
            before:content-[''] before:absolute
            before:left-0 before:top-[60px]
            before:w-0 before:h-[3px]
            before:bg-green-500 before:transition-all before:duration-300
            hover:before:w-full text-gray-600">
              Careers
            </a>
          </li>

        </ul>
        <a href="#"
           class="relative overflow-hidden
          bg-linear-to-bl from-green-500 to-cyan-500
          py-3 px-7 rounded-4xl inline-block
          before:content-[''] before:absolute before:inset-0
          before:bg-transparent
          before:transition-all before:duration-200
          hover:before:bg-gray-50/40 text-white">
          Request Invite
        </a>
      </nav>
      <button class="md:hidden" @click="open = !open">
        <img v-if="!open" src="/images/icon-hamburger.svg" alt="Menu"/>
        <img v-else src="/images/icon-close.svg" alt="Close"/>
      </button>
    </div>

    <div
        v-if="open"
        class="md:hidden bg-white rounded-lg shadow-lg mt-4 p-10"
    >
      <ul class="flex flex-col space-y-6 text-center">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
        <li><a href="#">Blog</a></li>
        <li><a href="#">Careers</a></li>
      </ul>

      <div class="text-center mt-6">
        <a href="#" class="bg-linear-to-bl from-green-500 to-cyan-500 py-3 px-7 rounded-4xl inline-block text-white">Request
          Invite</a>
      </div>
    </div>

  </header>
</template>