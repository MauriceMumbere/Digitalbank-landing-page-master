<script setup lang="ts">
</script>
<template>
  <section>
    <div class="flex flex-col-reverse md:flex-row md:justify-between h-screen items-center md:pl-32 px-8 py-6 md:px-0 md:py-0">

      <div class="flex-1 space-y-[2rem] text-center md:text-left">
        <h1 class="text-4xl md:text-[4rem] leading-14 md:leading-20">Next generation digital banking</h1>
        <p class="max-w-[27rem] text-gray-600"> Take your financial life online. Your Digitalbank account will be a one-stop-shop for
          spending, saving, budgeting, investing, and much more. </p>
        <div class=" pb-5">
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
        </div>
      </div>

      <div
          class="flex-2 bg-[url('/images/bg-intro-desktop.svg')] bg-cover bg-no-repeat bg-position-[right_-26rem_bottom_2.4rem]">
        <div class=" w-fit">
          <img class="md:ml-72 md:mt-16" src="/images/image-mockups.png" alt="Image mockups">
        </div>
      </div>

    </div>
  </section>
</template>