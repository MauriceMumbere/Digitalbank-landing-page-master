<script setup lang="ts">
defineProps({
  article : Object
})
</script>

<template>
    <div class="bg-white rounded-t-xl shadow-lg">
      <div>
        <div>
          <img class="h-[250px] rounded-t-xl" :src="article.image" alt="">
        </div>
        <div class="px-2 py-4">
          <div class="py-2">
            <h3>
              {{article.author}}
            </h3>
          </div>
          <div class="pb-2">
            <h2 class="font-bold text-xl">
              {{article.title}}
            </h2>
          </div>
          <p>
            {{article.description}}
          </p>
        </div>
      </div>
    </div>
</template>
