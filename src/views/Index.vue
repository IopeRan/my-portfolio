<script setup>
import Navbar from "../components/Navbar.vue"
import Home from "../components/HomeSec.vue"
import About from "../components/AboutSec.vue"
import TechStack from "../components/TechStackSec.vue"
import Project from "../components/ProjectSec.vue"
import Contact from "../components/ContactSec.vue"
import Footer from "../components/Footer.vue"
</script>
<template>
  <div class="w-full min-h-screen flex flex-col" style="font-family: 'Poppins', sans-serif">
    <Navbar></Navbar>
    <Home></Home>
    <About></About>
    <TechStack></TechStack>
    <Project></Project>
    <Contact></Contact>
    <Footer></Footer>
  </div>
</template>
