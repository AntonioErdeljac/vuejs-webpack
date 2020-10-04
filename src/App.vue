<template>
  <div>
    <h1>{{ title }}</h1>
    <users></users>
  </div>
</template>

<script>
import Users from './Users';

export default {
  components: {
    'users': Users,
  },
  data () {
    return {
      title: 'Vue App',
    }
  },
}
</script>

<style scoped>
h1 {
  color: purple;
}
</style>
