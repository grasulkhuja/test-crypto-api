<template>
  <div class="container">
    <nav class="nav">
      <div class="nav-left">
        <router-link
          class="brand"
          to="/">
          <wolfIcon width="30px"/>
        </router-link>

        <div class="tabs">
          <router-link exact-active-class="active" to="/">Exchanges</router-link>
          <router-link active-class="active" to="/markets">Markets</router-link>
          <router-link active-class="active" to="/trades">Trades</router-link>
          <router-link active-class="active" to="/chart">Chart</router-link>
        </div>
      </div>

      <div class="nav-right">
        <ThemeSwitch/>
      </div>
    </nav>
  </div>
</template>

<style>
  .nav {
    margin-bottom: 16px;
  }
  .nav-right {
    margin-right: 16px;
    align-items: center;
  }
</style>

<script>
import wolfIcon from '@/assets/svg/wolf-pack-battalion.svg'
import ThemeSwitch from '@/components/ThemeSwitch'

export default {
  name: 'Nav',
  components: {
    wolfIcon,
    ThemeSwitch
  },
  data () {
    return {}
  },
  computed: {},
  mounted () {
  },
  methods: {}
}
</script>
