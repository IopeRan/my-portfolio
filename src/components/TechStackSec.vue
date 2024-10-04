<template>
  <section id="techStack">
    <div class="bg-gray-200 pb-20 w-full min-h-screen">
      <h5 class="text-center py-6 text-xl lg:text-2xl font-medium">
        Tech Stack
      </h5>
      <div class="px-6 lg:px-8">
        <div class="grid grid-cols-2 lg:grid-cols-3 mt-5 gap-12 mx-12">
          <div v-for="stack in stacks" class="group" :key="stack">
            <div
              class="flex justify-center transition-all duration-100 bg-slate-100 items-center group-hover:bg-white grayscale group-hover:grayscale-0 py-6 h-52 lg:px-7 px-2 rounded-lg shadow-xl group-hover:border-[3px] group-hover:border-slate-300"
            >
              <img :src="stack.image" :width="stack.width" class="" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const stacks = [
  {
    title: "HTML5",
    image:
      "https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/120px-HTML5_logo_and_wordmark.svg.png",
    width: 150,
  },
  {
    title: "CSS3",
    image:
      "https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/CSS3_logo_and_wordmark.svg/100px-CSS3_logo_and_wordmark.svg.png",
    width: 110,
  },
  {
    title: "Javascript",
    image:
      "https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png",
    width: 120,
  },
  {
    title: "PHP",
    image:
      "https://upload.wikimedia.org/wikipedia/commons/thumb/2/27/PHP-logo.svg/1200px-PHP-logo.svg.png",
    width: 150,
  },
  {
    title: "Laravel",
    image:
      "https://logospng.org/download/laravel/logo-laravel-1024.png",
    width: 300,
  },
  {
    title: "VueJS",
    image:
      "https://cdn.sanity.io/images/8edntncj/production/7cb22a8a9885468d96662f6ece61ceb2bc95666d-500x300.png",
    width: 250,
  },
  {
    title: "TailwindCSS",
    image:
      "https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Tailwind_CSS_logo.svg/2560px-Tailwind_CSS_logo.svg.png",
    width: 290,
  },
  {
    title: "Bootstrap",
    image:
      "https://brandlogos.net/wp-content/uploads/2021/09/bootstrap-logo.png",
    width: 200,
  },

];
</script>
