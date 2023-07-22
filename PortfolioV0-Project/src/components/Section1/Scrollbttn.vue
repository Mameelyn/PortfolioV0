<template>
    <v-btn @click="scrollToTop" id="scrollToTopButton">
      <span class="material-symbols-outlined">
        stat_1
      </span>
    </v-btn>
</template>

<script>
export default {
  name: 'ScrollToTopButton',
  methods: {
    scrollToTop() {
      document.body.scrollTop = 0;
      document.documentElement.scrollTop = 0;
    }
  }
}
</script>

<style scoped>
#scrollToTopButton {
  position: fixed;
  bottom: 20px;
  right: 20px;
  padding: 10px;
  cursor: pointer;
  background-color: rosybrown;
  color: white;
  border-radius: 25px;
}
</style>