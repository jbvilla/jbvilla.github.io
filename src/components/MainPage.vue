<template>
  <AboutSection/>
  <EducationSection/>
  <SocialsSection/>
</template>

<script>
import EducationSection from "@/components/EducationSection.vue";
import AboutSection from "@/components/AboutSection.vue";
import SocialsSection from "@/components/SocialsSection.vue";

export default {
  name: "MainPage",
  components: {SocialsSection, AboutSection, EducationSection},

}
</script>

<style>

</style>