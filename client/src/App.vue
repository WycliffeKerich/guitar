<template>
  <div id="app">
    <v-app id="inspire">
      <page-header />
      <router-view/>
    </v-app>
  </div>
</template>

<script>
import PageHeader from '@/components/Header.vue'
export default {
  name: 'app',
  components: {
    PageHeader
  }
}
</script>

<style>
</style>
