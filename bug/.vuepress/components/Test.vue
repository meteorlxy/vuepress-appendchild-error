<template>
  <div v-if="test">
    test
  </div>
</template>

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
