<template>
  <ul>
    <li :key="user" v-for="user in users">{{user}}</li>
  </ul>
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
