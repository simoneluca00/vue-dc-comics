<template>
  <div id="app">

    <header>
      <div id="logoNav">
      <LogoComp />
      <NavComp />
      </div>
    </header>

    <main>
      <ContentComp />
      <InfoComp />
    </main>

    <footer>
      <FooterTopComp />
      <FooterBottomComp />
    </footer>

  </div>
</template>

<script>
import LogoComp from './components/LogoComp.vue'
import NavComp from './components/NavComp.vue'
import ContentComp from './components/ContentComp.vue'
import InfoComp from './components/InfoComp.vue'
import FooterTopComp from './components/FooterTopComp.vue'
import FooterBottomComp from './components/FooterBottomComp.vue'

export default {
  name: 'App',
  components: {
    LogoComp,
    NavComp,
    ContentComp,
    InfoComp,
    FooterTopComp,
    FooterBottomComp,
  }
}
</script>

<style lang="scss">

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  #logoNav {
    width: 85%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

}

</style>