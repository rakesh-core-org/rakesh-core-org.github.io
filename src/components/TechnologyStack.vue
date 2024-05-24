<template>
<v-data-table 
hover="true"
search
:headers="headers" :items="items" hide-default-footer="true">

    <template v-slot:item.logo="{ item }">
      
          <v-img
            :src="`https://cdn.vuetifyjs.com/docs/images/graphics/gpus/${item.logo}`"
            height="32"
            width="32"
            cover
          ></v-img>
   
      </template>

      <template v-slot:item.MyKnowledge="{ item }">
      
        <v-progress-linear
      bg-color="pink-lighten-3"
      color="lime"
      :model-value="item.MyKnowledge"
    ></v-progress-linear>

  </template>
      

</v-data-table>
</template>
<script setup>
  const headers = [
  { title: 'Logo', value: 'logo' },
  { title: 'Technology', value: 'Technology' },
  { title: 'Recently_worked_version', value: 'Recently_worked_version' },
  { title: 'MyKnowledge', value: 'MyKnowledge' },
  ]
  const items = [
    { 
        logo: '2.png',
      Technology: 'Kubernetes',
      Recently_worked_version: 'v1.5',
      MyKnowledge: '90'
    },

  ]
</script>

