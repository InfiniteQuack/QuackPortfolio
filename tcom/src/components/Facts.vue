<template>

  <div class="justify-center items-center">
    <h1 class="text-4xl Roboto">Fun Facts:</h1>
  </div>
  <div class="w-full flex items-center justify-start">
    <h1 class="text-4xl Roboto">{{ displayedText }}</h1>
  </div>

</template>

<script setup>
import { ref, onMounted } from 'vue';

const words = ["My dogs name is Jack, he's a corgi mix!", "I did an entire presentation on the Untitled Goose Game in high school. I got 100%",
  "When I slice cheese for a snack, my dog waits for me to offer him the rinds, if I don't, he starts rebelling.", "My favourite job so far has been working in a local cheese shop",
  "Cheese made in caves tends to develop richer and more complex flavours through a combination of factors like temperature, humidity and bacteria in the cave."
  ,"More than half of these facts are going to be about cheese",
  "A cyber attack occurs every 39 seconds.",
  "Cheese contains casein, which when digested, produces casomorphins, similar to opioids, that can bind to dopamine receptors. Meaning, cheese makes you happy!",
  "There are cheeses called triple cream cheese which has extra cream added to the milk, there's also triple milk cheeses that contain milk from three different animals (usually cow, goat and sheep!)",
  "There are currently over 1,300 programming languages in use worldwide."];
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