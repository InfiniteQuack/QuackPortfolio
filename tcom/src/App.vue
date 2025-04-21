<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Nav from "@/components/Nav.vue";
import Facts from "@/components/Facts.vue";
</script>

<template>

  <Nav></Nav>
  <h1 class="text-4xl Roboto pb-4 pt-4 justify-center flex pr-90">Juno Skutelnik</h1>
  <div id="about" class="justify-center flex flex-col Roboto items-center pb-5">
    <br><br>
    <img src="./assets/goosprof-Photoroom%20(2).png" alt="Profile Picture" width="273" height="281" class=""><br><br>
    <div class="w-2/6">
      What is up fellow computer enthusiasts, my name is Juno and I am soon to be a graduate of
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

  <div id="skills" class="items-center justify-center flex flex-col pb-6 mb-5 Roboto">
    <h1 class="text-4xl Roboto pb-4">My Skills</h1><br>
      <div class="grid grid-cols-3  gap-2  justify-center ">
        <button class="px-3 sm:px-4 py-2.5 sm:py-3 bg-[#000814] border border-[#000814]/20 rounded-lg  hover:border-[#5271ff] hover:shadow-[0_0_15px_rgba(82,113,255,0.3)] transition-all duration-300 text-left text-sm sm:text-base">
          System administration
        </button>
        <button class="px-3 sm:px-4 py-2.5 sm:py-3 bg-[#000814] border border-[#000814]/20 rounded-lg  hover:border-[#5271ff] hover:shadow-[0_0_15px_rgba(82,113,255,0.3)] transition-all duration-300 text-left text-sm sm:text-base">
          Front End Development
        </button>
        <button class="px-3 sm:px-4 py-2.5 sm:py-3 bg-[#000814] border border-[#000814]/20 rounded-lg  hover:border-[#5271ff] hover:shadow-[0_0_15px_rgba(82,113,255,0.3)] transition-all duration-300 text-left text-sm sm:text-base">
          Cloud Computing
        </button>
        <button class="px-3 sm:px-4 py-2.5 sm:py-3 bg-[#000814] border border-[#000814]/20 rounded-lg  hover:border-[#5271ff] hover:shadow-[0_0_15px_rgba(82,113,255,0.3)] transition-all duration-300 text-left text-sm sm:text-base">
          Blazor .NET
        </button>
        <button class="px-3 sm:px-4 py-2.5 sm:py-3 bg-[#000814] border border-[#000814]/20 rounded-lg  hover:border-[#5271ff] hover:shadow-[0_0_15px_rgba(82,113,255,0.3)] transition-all duration-300 text-left text-sm sm:text-base">
          REST API
        </button>
        <button class="px-3 sm:px-4 py-2.5 sm:py-3 bg-[#000814] border border-[#000814]/20 rounded-lg  hover:border-[#5271ff] hover:shadow-[0_0_15px_rgba(82,113,255,0.3)] transition-all duration-300 text-left text-sm sm:text-base">
          Git
        </button>
    </div>
  </div>

  <br><br>

  <div id="projects" class="items-center justify-center flex flex-col pb-5 mb-6 Roboto">
    <h1 class="text-4xl Roboto pb-2">Projects / Certificates</h1>

    <div class="grid grid-cols-3 gap-4">
      <div class="flex flex-wrap items-center mt-20 text-center">
        <div class="w-full md:w-3/5 lg:w-1/2 px-4">
          <img src="./assets/1000004853.jpg" alt="hackathon" class="inline-block rounded shadow-lg border border-merino-400 rotate-270">
        </div>
        <div class="w-full md:w-2/5 lg:w-1/2 px-4 text-center md:text-left lg:pl-12">
          <h3 class="font-bold mt-8 text-xl md:mt-0 sm:text-2xl">
            Sask Polytech Hackathon
          </h3>
          <p class="sm:text-lg mt-6">
            Participated in a two-day hackathon focused on creative tech solutions to improve
            Saskatchewan Polytechnic.<br><br>
            Developed an HTML and CSS-based form to increase accessibility on an online booking page.<br><br>
          </p>
        </div>
      </div>

      <div class="flex flex-wrap items-center mt-20 text-center">
        <div class="w-full md:w-3/5 lg:w-1/2 px-4">
          <img src="./assets/paradocs.png" alt="gem" class="inline-block rounded shadow-lg border border-merino-400">
        </div>
        <div class="w-full md:w-2/5 lg:w-1/2 px-4 text-center md:text-left lg:pl-12">
          <h3 class="font-bold mt-8 text-xl md:mt-0 sm:text-2xl">
            SaskPolytech Paradocs
          </h3>
          <p class="sm:text-lg mt-6">
            Developed a mobile and desktop application with Blazor .NET to assist in creating, viewing and managing learning
            materials for students and instructors of the Saskatchewan Polytechnic Paramedic program.
          </p>
        </div>
      </div>

      <div class="flex flex-wrap items-center mt-20 text-center">
        <div class="w-full md:w-3/5 lg:w-1/2 px-4">
          <img src="./assets/portfolio.png" alt="gem" class="inline-block rounded shadow-lg border border-merino-400">
        </div>
        <div class="w-full md:w-2/5 lg:w-1/2 px-4 text-center md:text-left lg:pl-12">
          <h3 class="font-bold mt-8 text-xl md:mt-0 sm:text-2xl">
            Portfolio Site
          </h3>
          <p class="sm:text-lg mt-6">
            Used vue and tailwinds css to create a custom website for displaying previous achievements and projects.
          </p>
        </div>
      </div>
    </div>
  </div>

  <Facts></Facts>
  <br><br><br><br><br><br>
  <div id="contact" class="items-center justify-center flex flex-col pb-5 mb-5 Roboto">
    <h1 class="text-4xl Roboto pb-2">Contact Information</h1>
    <p>Email: <a href="mailto:junomayes@gmail.com">junomayes@gmail.com</a></p>
    <p>LinkedIn: <a href="https://www.linkedin.com/in/juno-mayes-339642354/">Juno Skutelnik</a></p>
    <p>GitHub: <a href="https://github.com/InfiniteQuack">InfiniteQuack</a></p>
  </div>
</template>

<style scoped>

  @import url(
  "https://fonts.googleapis.com/css2?family=Roboto+Mono:ital,wght@0,100..700;1,100..700&display=swap"
  );

  .Roboto {
    font-family: 'Roboto Mono', sans-serif;
  }

</style>
