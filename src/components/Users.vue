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
  props: {
    users: {
      type: Array,
      required: true,
    },
  },
  data() {
    return {

    }
  },
}
</script>

<style scoped>

</style>
