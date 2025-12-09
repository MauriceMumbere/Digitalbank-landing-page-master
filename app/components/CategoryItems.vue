<script setup lang="ts">
  defineProps({
    category : Object
  })
</script>

<template>
    <div>
      <div class="flex items-center justify-center md:justify-start">
        <img :src="category.image" alt="">
      </div>
      <h3 class="py-8">{{category.title}}</h3>
      <p>{{category.description}}</p>
    </div>
</template>
