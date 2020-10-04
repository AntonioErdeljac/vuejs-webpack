<template>
  <div>
    <h1>List of Users</h1>
    <ul>
      <li :key="user" v-for="user in users">{{user}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data () {
    return {
      users: ['Antonio', 'Marko', 'Ivan']
    }
  }
}
</script>

<style scoped>
h1 {
  color: green;
}
</style>
