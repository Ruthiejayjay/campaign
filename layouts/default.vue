<template>
  <div v-if="alphineready">
      <c-nav />

      <nuxt />

      <c-footer />
  </div>
</template>

<script>
import CFooter from '~/components/cFooter.vue'
import cNav from '~/components/cNav.vue'
export default {
  components: { cNav, CFooter },
     data() {
    return {
      alphineready: false,
    };
  },

  head() {
    return {
      title: "Imumolen", // Other meta information
      script: [
        {
          hid: "alphine",
          src: "https://cdnjs.cloudflare.com/ajax/libs/alpinejs/2.8.0/alpine.js",
          // Changed after script load
          callback: () => {
            this.alphineready = true;
          },
        },
      ],
    };
  },
}
</script>

<style>

</style>