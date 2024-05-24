<template>
    <v-container>
      <v-row no-gutters>
        <v-col
          cols="12"
          sm="4"
        >
          <v-sheet class="ma-2 pa-2">
            <EverydaySchedule />
          </v-sheet>
        </v-col>

        <v-col
          cols="12"
          sm="4"
        >
          <v-sheet class="ma-2 pa-2">
            <Awards />
          </v-sheet>
        </v-col>

        <v-col
          cols="12"
          sm="4"
        >
          <v-sheet class="ma-2 pa-2">
            <CoreSkills />
          </v-sheet>
        </v-col>

      </v-row>
    </v-container>
  </template>

<script setup>
import EverydaySchedule from './EverydaySchedule.vue'
import Awards from './Awards.vue'
import CoreSkills from './CoreSkills.vue'
</script>