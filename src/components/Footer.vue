<template>
    <div class="w-full px-6 pb-6 flex flex-col lg:flex-row lg:justify-between">
        <div class="animate-bounce font-semibold text-lg">Erlang</div>
        <ul class="hidden lg:flex lg:flex-row lg:gap-6">
            <li v-for="section in sections" :key="section.name">
                <a :href="section.href" class="hover:border-b hover:border-b-black hover:duration-150">{{ section.name }}</a>
            </li>
        </ul>
    </div>
</template>

<script setup>

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