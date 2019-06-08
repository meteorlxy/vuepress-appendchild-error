<div v-if="test" />

<script>
export default {
  data: () => ({
    test: false,
  }),

  beforeMount () {
    this.test = true
  },
}
</script>