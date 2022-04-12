<template>
  <div id="app">
    <header>
      <div id="logoNav">
      <LogoComp />
      </div>
    </header>
  </div>
</template>

<script>
import LogoComp from './components/LogoComp.vue'

export default {
  name: 'App',
  components: {
    LogoComp,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  header {
    padding: 20px 0;

    #logoNav {
      width: 80%;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
  }

}

</style>
