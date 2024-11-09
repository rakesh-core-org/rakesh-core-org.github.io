<template>
  <v-app>
    <v-main>
      <MainContent />
    </v-main>

    <AppFooter />
  </v-app>
</template>

<script setup>
  //
</script>

<style>
.v-theme--dark {
    .v-table {
    background: rgb(18,18,18)

    }
    .v-card--variant-elevated, .v-card--variant-flat {
    background: rgb(18,18,18);
    color: rgba(var(--v-theme-on-surface), var(--v-high-emphasis-opacity));
}
}


</style> 