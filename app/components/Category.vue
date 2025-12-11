<script setup lang="ts">
const categories = [
  {
    id: 1,
    image : "images/icon-online.svg",
    title : "Online Banking",
    description :"Our modern web and mobile applications allow you to keep track of your finances wherever you are in the world.",
  },
  {
    id: 2,
    image : "images/icon-online.svg",
    title : "Simple Budgeting",
    description :"See exactly where your money goes each month. Receive notifications when you’re close to hitting your limits.",
  },
  {
    id: 3,
    image : "images/icon-online.svg",
    title : "Fast Onboarding",
    description :"We don’t do branches. Open your account in minutes online and start taking control of your finances right away.",
  },
  {
    id: 4,
    image : "images/icon-online.svg",
    title : "Open API",
    description :"Manage your savings, investments, pension, and much more from one account. Tracking your money has never been easier.",
  },
]
</script>

<template>
    <div class="px-8 py-6 md:px-[8rem] md:py-[5rem] bg-gray-100 text-center md:text-left">
      <h2 class="text-4xl pb-[3rem]">Why choose Digitalbank?</h2>
      <p class="max-w-[40rem] mb-[5rem]">We leverage Open Banking to turn your bank account into your financial hub. Control
        your finances like never before.
      </p>
      <div class="grid grid-cols-1 md:grid-cols-4 gap-20">
        <div v-for="category in categories" :key="category.id">
          <CategoryItems :category="category" />
        </div>
      </div>
    </div>
</template>
