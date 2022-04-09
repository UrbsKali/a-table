<template>
    <Sidebar />
    <Card :icon="bx-lemon" :title="Broda" :description="Oya" />
</template>

<script>
import Sidebar from "../components/sidebar.vue";
import Card from "../components/card.vue";
export default {
    name: 'component.vue',
    components: {Sidebar, Card},
    data() {
      return {}
    }
  }
</script>

<style>

</style>