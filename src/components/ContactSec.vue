<template>
  <section id="contact" class="flex justify-center items-center pb-12">
    <div
      class="w-full flex p-6 justify-center flex-col max-w-md bg-slate-200 rounded-md shadow-lg"
    >
      <div class="">
        <h3 class="text-3xl font-bold font-mono">My Contact</h3>
      </div>
      <div v-for="contact in contacts" :key="index" class="flex gap-5 mt-5">
        <div class="flex">
          <i
            class="text-black font-bold text-2xl transition-all duration-300"
            :class="contact.icon"
          ></i>
        </div>
        <div class="">
          <h3 class="text-xl">{{ contact.text }}</h3>
          <a class="font-bold text-xl">{{ contact.contact }}</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const contacts = [
    {
        text: 'email',
        contact: 'chilliope48@gmail.com',
        icon: 'fa-solid fa-envelope',
    },
    {
        text: 'instagram',
        contact: '@lang_andp',
        icon: 'fa-brands fa-instagram'
    }
]
</script>