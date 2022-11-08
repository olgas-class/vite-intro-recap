<script>
import AppBanner from "./components/AppBanner.vue";

export default {
  data() {
    return {
      title: "Mio titolo"
    }
  },
  components: {
    AppBanner
  }
}
</script>

<template>
  <section>
    <h1>{{ title }}</h1>
  </section>
  <AppBanner />
</template>

<style>
h1 {
  color: blue;
}

h2 {
  color: brown;
}
</style>