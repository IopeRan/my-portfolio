<template>
  <nav
    class="bg-slate-100 w-full h-max text-black font-medium flex flex-row justify-between px-6 py-3"
    style="font-family: 'Poppins', sans-serif"
  >
    <div class="flex flex-row gap-1 font-semibold text-lg">
      <div>Erlang</div>
      <div class="text-violet-500">Andriyanputra</div>
    </div>
    <ul class="hidden lg:flex lg:flex-row gap-8">
      <li v-for="section in sections" :key="section.name">
        <a :href="section.href">{{ section.name }}</a>
      </li>
    </ul>
    <button class="lg:hidden text-2xl" @click="showElement"><i class="fa-solid fa-bars"></i></button>
    <div v-if="isElementVisible" class="bg-white w-max h-max rounded-lg text-black absolute right-6 top-12 pl-3 pr-20 py-2" >
        <ul class="flex flex-col gap-2 w-full">
          <li v-for="section in sections" :key="section.name">
            <a :href="section.href">{{ section.name }}</a>
          </li>
        </ul>
      </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue';

const isElementVisible = ref(false);

function showElement() {
  isElementVisible.value = !isElementVisible.value;
}

const sections = [
  {
    href: "#home",
    name: "Home",
  },
  {
    href: "#about",
    name: "About",
  },
  {
    href: "#techStack",
    name: "Tech Stack",
  },
  {
    href: "#project",
    name: "Project",
  },
  {
    href: "#contact",
    name: "Contact",
  },
]

</script>
