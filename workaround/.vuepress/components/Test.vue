<template>
  <div v-if="test">
    test
  </div>

  <div v-else />
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
