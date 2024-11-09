<template>
    <v-container>
      <h2> What are my 4 quadrant skills</h2>
      <v-row no-gutters>
        <v-col>
          
            <DevopsKnowledge />
          
        </v-col>
        <v-col>
          
            <CloudKnowledge />
        
        </v-col>
  
        <v-responsive width="100%"></v-responsive>
  
        <br />
        <v-col>
          
            <SystemAdministrationKnowledge />
          
        </v-col>
  
        <v-col>
          
            <ArtificialIntelligenceKnowledge />
          
        </v-col>
      </v-row>
    </v-container>
  </template>

<script>
import DevopsKnowledge from './DevopsKnowledge.vue'
import CloudKnowledge from './CloudKnowledge.vue'
import SystemAdministrationKnowledge from './SystemAdministrationKnowledge.vue'
import ArtificialIntelligenceKnowledge from './ArtificialIntelligenceKnowledge.vue'
</script>