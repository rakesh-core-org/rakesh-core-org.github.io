<template>

<v-alert
    v-model="alert"
    text="You are viewing the recent version of my profile"
    title="Autoclose"
    type="info"
    variant="tonal"
    closable
  ></v-alert>
  
</template>

<script>

export default {
  data() {
    return {
      alert: true
    }
  },
  created(){
    setTimeout(()=>{
      this.alert=false
    },5000)
  }

}

</script>