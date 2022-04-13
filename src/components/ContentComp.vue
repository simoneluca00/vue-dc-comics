<template>
  <div class="container">
      <div id="content">
          --> QUI VA INSERITO IL CONTENUTO
      </div>
  </div>
</template>

<script>
export default {
  name: 'ContentComp',

}
</script>

<style scoped lang="scss">
@import '../style/variabili.scss';

.container {
    background-color: $bg-dark;
    padding: 50px 0;

    #content {
        width: 85%;
        margin: 0 auto;
        text-align: center;
        color: $text-white;
    }
}

</style>