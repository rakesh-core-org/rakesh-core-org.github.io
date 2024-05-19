<template>
    <v-app-bar :elevation="2" rounded>
      <v-app-bar-title>Rakesh Nagarajan</v-app-bar-title>
      
      <v-tooltip text="Theme" location="bottom">
        <template v-slot:activator="{ props }">
          <v-btn
            v-bind="props"
            color="black"
            size="large"
            :prepend-icon="mdiWeatherSunny"
            v-if="theme.global.name.value === 'light'"
            @click="toggleTheme"
          ></v-btn>
          <v-btn
          v-bind="props"
          color="white"
            size="large"
            :prepend-icon="mdiWeatherNight"
            v-if="theme.global.name.value === 'dark'"
            @click="toggleTheme"
          ></v-btn>
        </template>
      </v-tooltip>
      <opensource-projects />
    </v-app-bar>
  </template>
  
  <script>
  import OpensourceProjects from './OpensourceProjects.vue'
  import { useTheme } from 'vuetify'
  import { mdiWeatherSunny } from "@mdi/js";
  import { mdiWeatherNight } from "@mdi/js";

  export default {
    components: {
      OpensourceProjects,

    },
    data: () => ({
      mdiWeatherSunny,
      mdiWeatherNight,
    }),
    setup() {
  const theme = useTheme()
  return {
    theme,
    toggleTheme: () =>
        (theme.global.name.value = theme.global.current.value.dark
          ? "light"
          : "dark"),
  }

    }
  // function toggleTheme () {
  //   theme.global.name = theme.global.current.dark ? 'light' : 'dark'
  // }

}
  </script>