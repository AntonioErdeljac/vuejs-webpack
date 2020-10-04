<template>
  <div>
    <h1>{{ title }}</h1>
    <p>{{ greeting() }}</p>
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'Hello vue-cli',
    }
  },
  methods: {
    greeting () {
      return 'Hello World'
    }
  }
}
</script>

<style>

</style>
