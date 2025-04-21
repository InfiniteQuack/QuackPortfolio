<template>

  <div class="justify-center items-center">
    <h1 class="text-4xl Roboto">Fun Facts:</h1>
  </div>
  <div class="w-2/6 flex items-center justify-start">
    <h1 class="text-4xl Roboto">{{ displayedText }}</h1>
  </div>

</template>

<script setup>
import { ref, onMounted } from 'vue';

const words = ["Hello, World! this is a really liong sdfljkasdkdf sadjfas dfsa df sadf sdf sa df asdf sa df asdf as df as df asdf as df asdf", "Welcome to my website!", "This is a typewriter effect."];
const displayedText = ref("");
let i = 0;
let j = 0;
let isDeleting = false;

function type() {
  const currentWord = words[i];

  if (isDeleting) {
    displayedText.value = currentWord.substring(0, j - 1);
    j--;
    if (j === 0) {
      isDeleting = false;
      i = (i + 1) % words.length;
    }
  } else {
    displayedText.value = currentWord.substring(0, j + 1);
    j++;
    if (j === currentWord.length) {
      isDeleting = true;
    }
  }

  setTimeout(type, 100);
}

onMounted(() => {
  type();
});
</script>

<style scoped>
  @import url(
  "https://fonts.googleapis.com/css2?family=Roboto+Mono:ital,wght@0,100..700;1,100..700&display=swap"
  );

  .Roboto {
    font-family: 'Roboto Mono', sans-serif;
  }

</style>