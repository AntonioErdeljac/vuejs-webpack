<template>
  <div id="users">
    <ul>
      <li :key="user.name" v-for="user in users" @click="user.visible = !user.visible">
        <h2>{{ user.name }}</h2>
        <h3 v-show="user.visible">{{ user.job }}</h3>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data () {
    return {
      users: [{
        name: 'Antonio',
        job: 'Software engineer',
        visible: false,
      }, {
        name: 'Marko',
        job: 'Dev ops',
        visible: false,
      }, {
        name: 'Ivan',
        job: 'Project manager',
        visible: false,
      }]
    }
  }
}
</script>

<style scoped>

</style>
