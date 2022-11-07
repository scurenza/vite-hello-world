<script>
import AppTitle from "./components/AppTitle.vue";
import AppBanner from "./components/AppBanner.vue";

export default {
  data() {
    return {
      greeting: "Ciao mondo!"
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
  <h1>{{ AppTitle }}</h1>
  <section>
    <AppTitle />
    <AppBanner />
  </section>
  <button @click="saluta">Saluta</button>
</template>

<style>
h1 {
  color: red;
}
</style>