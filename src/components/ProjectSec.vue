<template>
  <section id="project">
    <div class="bg-white w-full min-h-screen pb-20">
      <h5 class="text-center py-6 text-xl lg:text-2xl font-medium">
        My Project
      </h5>
      <div
        class="grid grid-cols-1 place-items-center lg:grid-cols-2 mt-5 gap-12 mx-12"
      >
        <div v-for="project in projects" class="group block" :key="index">
          <div
            class="transition-all lg:w-[30vw] flex-col duration-100 bg-white items-center rounded-lg"
          >
            <div class="">
              <div class="flex justify-center items-center relative">
                <img :src="project.image" class="rounded-lg" alt="" />
                <div
                  class="absolute z-10 group-hover:z-30 opacity-0 group-hover:opacity-100 rounded-md bg-[#6e6d6d8a] w-full h-full flex justify-center items-center duration-300 transition-opacity"
                >
                  <div class="flex">
                    <a :href="project.github" target="_blank" class="font-bold text-4xl"
                      ><i
                        class="fa-brands fa-github text-white hover:text-black transition-colors duration-200"
                      ></i
                    ></a>
                  </div>
                </div>
              </div>
              <div class="flex flex-col mt-5 justify-center items-center">
                <h3 class="text-center text-3xl font-bold   ">
                  {{ project.title }}
                </h3>
                <p class="font-sans text-center text-slate-600">
                  {{ project.desc }}
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>

const projects = [
  {
    title: "Techno Cashier",
    desc: "Techno Cashier adalah aplikasi berbasis website yang memudahkan kasir dan pembeli melakukan transaksi.",
    github: 'https://github.com/IopeRan/aplikasi-kasir-techno.git',
    image:
      "techno.png",
  },
  {
    title: "E-Profile Students",
    desc: "E-Profile Students adalah website berisi tes untuk mengetahui karakter siswa siswa sekolah.",
    github: 'https://github.com/RepublikKode/E-Profile-Student',
    image:
      "e-profile.png",
  },
  {
    title: "Elibin",
    desc: "E-Library Information digunakan untuk mempermudah dalam mencari informasi, data dan juga mempermudah managemen sistem perpustakaan.",
    github: 'https://github.com/E-LibraryInformation/Elibin-DevStage',
    image:
      "elibin.png",
  },
  {
    title: "Web OSIS",
    desc: "Web OSIS SMKN 2 Banjarmasin dibuat untuk mempermudah absensi dan memberikan informasi via forum.",
    github: 'https://github.com/IopeRan/OsisSkendaBjm',
    image:
      "osis.png",
  },
]

</script>
