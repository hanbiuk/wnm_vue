<template>
    <home-header></home-header>
</template>

<script>
import HomeHeader from './components/Header'
export default {
  name: 'Home',
  components: {
    HomeHeader
  },
  activated () {
    this.getProfilePhote()
  }
}
</script>

<style>
</style>
