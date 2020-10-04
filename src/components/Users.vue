<template>
  <div id="users">
    <ul>
      <li :key="user.name" v-for="user in users" @click="user.visible = !user.visible">
        <h2>{{ user.name }}</h2>
        <h3 v-show="user.visible">{{ user.job }}</h3>
      </li>
    </ul>
    <button @click="deleteUser">Delete one</button>
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
  methods: {
    deleteUser() {
      this.users.pop();
    }
  },
  beforeCreate() {
    alert('Before creation.')
  },
  created() {
    alert('Created.')
  },
  beforeMount() {
    alert('Before mount.')
  },
  mounted() {
    alert('Mounted.')
  },
  beforeUpdate() {
    alert('Before update.')
  },
  updated() {
    alert('Updated.')
  }
}
</script>

<style scoped>

</style>
