<template>
  <div>
    <app-header v-on:changeTitle="updateTitle($event)" :title="title"></app-header>
    <users :users="users"></users>
    <app-footer :title="title"></app-footer>
  </div>
</template>

<script>
import Footer from './components/Footer';
import Header from './components/Header';
import Users from './components/Users';

export default {
  components: {
    'app-header': Header,
    'app-footer': Footer,
    'users': Users,
  },
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
      }],
      title: 'Vue Users',
    }
  },
  methods: {
    updateTitle(event) {
      this.title = event;
    }
  }
}
</script>

<style>
</style>
