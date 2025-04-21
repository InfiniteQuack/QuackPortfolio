<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Nav from "@/components/Nav.vue";
import Facts from "@/components/Facts.vue";
</script>

<template>

  <Nav></Nav>
  <div id="about" class="justify-center flex flex-col Roboto items-center pb-5">
    <br><br>
    <img src="./assets/goosprof.png" alt="Profile Picture" width="273" height="281" class=""><br><br>
    <div class="w-2/6">
      What is up fellow computer enthusiasts, my name is Juno I am soon the be a graduate of
      Sask Polytech's Computer Systems Technology Program. So far, my favourite aspect of
      computer science has been web design. I now have over two years of experience with
      web development and I'm passionate about making designs that are user friendly, intuitive, and have a little silliness.
      <br><br>
      Other than web developing I love learning about cyber security and how different vulnerabilities
      have been found, used, and solved. I especially enjoy the stories from the <a href="https://darknetdiaries.com/">DarkNet Diaries</a>
      and hearing from people who actually work in industry.
      <br><br>
      After graduation I plan on expanding my knowledge on cyber security and am currently working on gaining my CPTS certificate.
      <br><br>
      <br><br>

    </div>
  </div>

  <div id="skills" class="items-center justify-center flex pb-5">
    <h1 class="text-4xl Roboto">My Skills</h1>
  </div>

  <div id="projects" class="items-center justify-center flex flex-col pb-5">
    <h1 class="text-4xl Roboto">Projects / Certificates</h1>

    <div class="grid grid-cols-3 gap-4">
      <div class="...">01</div>
      <div class="...">02</div>
      <div class="...">03</div>
      <div class="col-span-2 ...">04</div>
      <div class="...">05</div>
      <div class="...">06</div>
      <div class="col-span-2 ...">07</div>
    </div>
  </div>
  <div id="contact">

  </div>
  <Facts></Facts>


</template>

<style scoped>

  @import url(
  "https://fonts.googleapis.com/css2?family=Roboto+Mono:ital,wght@0,100..700;1,100..700&display=swap"
  );

  .Roboto {
    font-family: 'Roboto Mono', sans-serif;
  }

</style>
