<script>
import AppTitle from "./components/AppTitle.vue";
import AppBanner from "./components/AppBanner.vue";

export default {
  data() {
    return {

    }
  },
  components: {
    AppTitle,
    AppBanner
  },
  methods: {
    saluta() {
      alert("ciao");
    }
  }
}
</script>

<template>
  
  <section>
    <AppTitle />
    <AppBanner />
  </section>
  <button @click="saluta">Saluta</button>
</template>

<style>
h1 {
  color: orange;
}
</style>