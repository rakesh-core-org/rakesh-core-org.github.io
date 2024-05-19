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
        <v-row
          justify="space-around"
          no-gutters
        >
          phone|email|github|linkedin|location
        </v-row>
      </v-expansion-panel-text>
    </v-expansion-panel>
    </v-expansion-panels>



</template>