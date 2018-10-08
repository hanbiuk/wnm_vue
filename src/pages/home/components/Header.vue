<template>
  <b-navbar toggleable="md" type="dark" variant="dark " fixed="top">

    <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

    <b-navbar-brand class="header-brand-logo" href="#">
      <img class="header-logo" :src="leftLogo" alt="wnm" >
    </b-navbar-brand>

    <b-collapse is-nav id="nav_collapse">

      <b-navbar-nav>
        <b-nav-item href="#">WeNeverMe</b-nav-item>
        <b-nav-item href="#">我不是猫</b-nav-item>
        <b-nav-item href="#">我不是佟离</b-nav-item>
        <b-nav-item href="#" active="true">我不是江小白</b-nav-item>
      </b-navbar-nav>

      <b-navbar-nav class="ml-auto">

        <b-navbar-brand class="header-brand-profile" href="#">
          <img class="header-profile" :src="profilePhoto" alt="me" >
        </b-navbar-brand>

      </b-navbar-nav>

    </b-collapse>

    <b-navbar-brand class="header-brand-playing" href="#">
      <img class="header-playing" :src="profilePhoto" alt="playing" >
    </b-navbar-brand>
    <!--TODO: 手机屏幕点击导航后，会把这个按钮也收进去-->

  </b-navbar>
</template>

<script>
export default {
  name: 'HomeHeader',
  data () {
    return {
      leftLogo: require('@/assets/imgs/logo2.png'),
      profilePhoto: '/static/logo4.png'
    }
  }
}
</script>

<style lang="stylus" scoped>
  .header-brand-logo
    margin: 0
    padding: 0
    position: relative
    overflow: hidden
    width: 40px
    height: 40px
    .header-logo
      width: 100%
      height: 100%
  .header-brand-profile
    margin: 0
    padding: 0
    position: relative
    overflow: hidden
    width: 40px
    height: 40px
    .header-profile
      margin: 0
      padding: 15%
      width: 100%
      height: 100%
  .header-brand-playing
    margin: 0
    padding: 0
    position: relative
    overflow: hidden
    width: 40px
    height: 40px
    .header-playing
      margin: 0
      padding: 15%
      width: 100%
      height: 100%
</style>
