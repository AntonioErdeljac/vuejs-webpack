<template>
  <header>
    <h1 @click="changeTitle">{{ title }}</h1>
  </header>
</template>

<script>
import { bus } from '../main';

export default {
  props: {
    title: {
      type: String,
      required: true,
    },
  },
  methods: {
    changeTitle() {
      this.title = 'Vue Test'
      bus.$emit('titleChanged', 'Vue Test')
    }
  }
}
</script>

<style scoped>
  header {
    background: lightgreen;
    padding: 10px;
  }
  h1 {
    color: #222;
    text-align: center;
  }
</style>
