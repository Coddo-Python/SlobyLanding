<template>
  <img src="/images/Star.svg" class="w-2 absolute top-0 left-0" :style="{'top': top, 'left': left}" alt="Star">
</template>

<script>
export default {
  name: "Star",
  data () {
    return {
      top: Math.random() * 100 + 'vh',
      left: Math.random() * 100 + 'vw',
    }
  },
  methods: {
    onMouseMove(e) {
      const x = e.clientX / window.innerWidth
      const y = e.clientY / window.innerHeight
      this.$el.style.transform = 'translate(-' + x * 50 + 'px, -' + y * 50 + 'px)'
    }
  },
  mounted () {
    window.addEventListener('mousemove', this.onMouseMove)
  },
}
</script>

<style scoped>

</style>
