<template>
  <div  data-bs-spy="scroll" data-bs-target="#header-bar" data-bs-offset="0" class="scrollspy-example" tabindex="0">
    <div id="heroSection">
      <HeroComponent></HeroComponent>
    </div>
    <div id="aboutMeSection" class="py-3 bg-dark text-white">
      <AboutMeComponent></AboutMeComponent>
    </div>
    <div id="servicesSection" class="py-3 bg-dark text-white">
      <ServicesComponent></ServicesComponent>
    </div>
    <div id="experienceSection" class="py-3 bg-dark text-white">
      <ExperienceComponent></ExperienceComponent>
    </div>
  </div>

</template>

<style>

</style>

<script>
import HeroComponent from "../components/HeroComponent.vue";
import AboutMeComponent from "../components/AboutMeComponent.vue";
import ServicesComponent from "../components/ServicesComponent.vue";
import ExperienceComponent from "../components/ExperienceComponent.vue";

export default{
  components :{ HeroComponent, AboutMeComponent , ServicesComponent, ExperienceComponent }
}

</script>