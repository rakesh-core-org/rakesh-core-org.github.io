<template>
  <v-container>
    <app-bar />
    
    <!-- <ExperienceCounter /> -->
    <contact-me />
    <acknowledge />
    <AboutMe />
    <my-timeline />
    <!-- <ThirdSection /> -->
    <br />

    <FifthSection />
    <SixthSection />
    
    <hr />
    <Declaration />
    <br />
    <OpensourceProjects />
    <!-- <v-btn position="fixed" location="bottom right" class="ma-4" size="large" icon="mdi-meni" /> -->
  </v-container>
</template>

<script setup>
import AppBar from './AppBar.vue'
import Acknowledge from './Acknowledge.vue'
import MyTimeline from './MyTimeline.vue'
import AboutMe from './AboutMe.vue'
import ThirdSection from './ThirdSection.vue'
import OpensourceProjects from './OpensourceProjects.vue'
import ContactMe from './ContactMe.vue'
import FifthSection from './FifthSection.vue'
import SixthSection from './SixthSection.vue'
import Declaration from './Declaration.vue'
import ExperienceCounter from './ExperienceCounter.vue'
</script>

