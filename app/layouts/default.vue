<script setup lang="ts">
useHead({
  title: "Frontend Mentor | Loopstudios landing page",
  link: [
    {
      rel: "icon",
      type: "image/png",
      sizes: "32x32",
      href: "/images/favicon-32x32.png",
    },
  ],
});
</script>

<template>
  <div>
    <Header />
    <slot />
    <Footer />
  </div>
</template>
