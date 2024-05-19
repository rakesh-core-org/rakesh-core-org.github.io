<template>
  <v-container>
    <app-bar />
    <acknowledge />
    <contact-me />
    <my-timeline />
  </v-container>
</template>

<script setup>
import AppBar from './AppBar.vue'
import Acknowledge from './Acknowledge.vue'
import MyTimeline from './MyTimeline.vue'
import ContactMe from './ContactMe.vue'
</script>
