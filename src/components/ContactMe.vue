<template>
  <v-expansion-panels>
    <v-expansion-panel>
      <v-expansion-panel-title v-slot="{ expanded }">
        <v-row no-gutters>
          <v-col class="d-flex justify-start" cols="4">
            Reach me
          </v-col>

        </v-row>
      </v-expansion-panel-title>
      <v-expansion-panel-text>
        <v-row justify="space-around" no-gutters>
          <v-col cols="10" sm="2">
            <v-btn :prepend-icon="mdiPhone" variant="plain" href="" target="_blank">
              REDACTED
            </v-btn>
          </v-col>
          <v-col cols="10" sm="2">


            <v-btn :prepend-icon="mdiEmailBox" variant="plain" href="" target="_blank">
              REDACTED
            </v-btn>
          </v-col>

          <v-col cols="10" sm="2">
            <v-btn :prepend-icon="mdiGithub" variant="plain" href="https://github.com/RakeshNagarajanOrg"
              target="_blank">
              github
            </v-btn>


          </v-col>

          <v-btn :prepend-icon="mdiLinkedin" variant="plain" href="https://www.linkedin.com/in/rakesh-nagarajan/"
            target="_blank">
            linkedin
          </v-btn>

        </v-row>
      </v-expansion-panel-text>
    </v-expansion-panel>
  </v-expansion-panels>



</template>

<script>
import { mdiPhone } from '@mdi/js';
import { mdiEmailBox } from '@mdi/js';
import { mdiGithub } from '@mdi/js';
import { mdiLinkedin } from '@mdi/js';

export default {
  data() {
    return {
      mdiPhone,
      mdiEmailBox,
      mdiGithub,
      mdiLinkedin

    }
  }
}


</script>