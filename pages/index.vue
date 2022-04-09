<template>
    <Sidebar />
    <Card :icon_is_bx="false" :icon="'📜'" :title="'Broda'" :description="'Oya'" />
</template>

<script>
import Sidebar from "../components/sidebar.vue";
import Card from "../components/card.vue";
export default {
    name: 'component.vue',
    components: {Sidebar, Card},
    data() {
      return {

      }
    }
  }
</script>

<style>
body{
  background-color: #272543;
}
</style>