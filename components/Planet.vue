<template>
  <img class="hidden lg:block absolute z-10" alt="Planet">
</template>

<script>
export default {
  name: "Planet",
  methods: {
    onMouseMove(e) {
      const x = e.clientX / window.innerWidth
      const y = e.clientY / window.innerHeight
      this.$el.style.transform = 'translate(-' + x * 10 + 'px, -' + y * 10 + 'px)'
    }
  },
  mounted () {
    window.addEventListener('mousemove', this.onMouseMove)
  },
}
</script>

<style scoped>

</style>
