<template>
  <v-container>
    <h2>Whats in my brain?</h2>
    <v-row>
      <v-col>

        <h3>Primary Skills</h3>
        <TechnologyStackPrimary />

      </v-col>

      <v-col>

        <h3>Secondary Skills</h3>
        <TechnologyStackSecondary />

      </v-col>

    </v-row>

    <v-row>
      <v-col cols="6">
    <v-expansion-panels>
          <v-expansion-panel>
            <v-expansion-panel-title>View my Tertiary Skills too </v-expansion-panel-title>
            <v-expansion-panel-text>

        <h3>Tertiary Skills</h3>
        <TechnologyStackTertiary />
      </v-expansion-panel-text>
      </v-expansion-panel>
    </v-expansion-panels>
  </v-col>
</v-row>

  </v-container>
</template>

<script>
import TechnologyStackPrimary from './TechnologyStackPrimary.vue'
import TechnologyStackSecondary from './TechnologyStackSecondary.vue'
import TechnologyStackTertiary from './TechnologyStackTertiary.vue'

</script>