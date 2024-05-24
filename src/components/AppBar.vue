<template>
  <v-app-bar :elevation="2" rounded>
    <v-app-bar-title>Rakesh Nagarajan</v-app-bar-title>
    <template v-slot:append>
      <!-- <opensource-projects /> -->
    </template>

    <v-tooltip text="Theme" location="bottom">
      <template v-slot:activator="{ props }">
        <v-btn v-bind="props" color="black" size="large" :prepend-icon="mdiWeatherSunny"
          v-if="theme.global.name.value === 'light'" @click="toggleTheme"></v-btn>
        <v-btn v-bind="props" color="white" size="large" :prepend-icon="mdiWeatherNight"
          v-if="theme.global.name.value === 'dark'" @click="toggleTheme"></v-btn>
      </template>
    </v-tooltip>


    <v-tooltip text="Download">
      <template v-slot:activator="{ props }">
        <v-btn :prepend-icon="mdiDownload" v-bind="props" @click.prevent="downloadofflinefile()"></v-btn>
      </template>
    </v-tooltip>


  </v-app-bar>
</template>

<script>
// import OpensourceProjects from './OpensourceProjects.vue'
import { useTheme } from 'vuetify'
import { mdiWeatherSunny } from "@mdi/js";
import { mdiWeatherNight } from "@mdi/js";
import { mdiDownload } from '@mdi/js';

import axios from 'axios';

export default {
  components: {
    // OpensourceProjects,

  },
  data: () => ({
    mdiWeatherSunny,
    mdiWeatherNight,
    mdiDownload,
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

  },
  methods: {
    downloadofflinefile(){
      console.log("Download starts...")
      axios.get('https://github.com/RakeshNagarajanOrg/RakeshNagarajanOrg.github.io/blob/main/public/favicon.ico', { responseType: 'blob' })
      .then(response => {
        const blob = new Blob([response.data], { type: 'application/pdf' })
        const link = document.createElement('a')
        link.href = URL.createObjectURL(blob)
        link.download = label
        link.click()
        URL.revokeObjectURL(link.href)
      }).catch(console.error)
    }
  },

}
</script>