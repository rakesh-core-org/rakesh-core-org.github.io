<template>
    <div>
        <v-checkbox v-model="selected" value="info" color="blue" density="compact"  hide-details label="All above given information were true. You can trust me."></v-checkbox>
        <v-checkbox v-model="selected" value="relocate" color="blue" density="compact" hide-details label="Ready to relocate based on project demand."></v-checkbox>
        <v-checkbox v-model="selected" value="shift" color="blue" density="compact" hide-details label="Open to work in shift based on project demand."></v-checkbox>
        <br>
        Place	: Coimbatore
        <br>		
        Date	: {{currentDate()}}

    </div>
</template>

<script>
export default {
    data () {
      return {
        selected: ['info','relocate','shift'],
      }
    },
  methods: {
    currentDate() {
      const current = new Date();
      const date = `${current.getDate()}/${current.getMonth()+1}/${current.getFullYear()}`;
      return date;
    }
  }
};
</script>