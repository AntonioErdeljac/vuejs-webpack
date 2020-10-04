<template>
  <div>
    <app-header></app-header>
    <users></users>
    <app-footer></app-footer>
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
    }
  },
}
</script>

<style>
</style>
