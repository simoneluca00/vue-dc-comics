<template>
  <div class="container">
      <div class="row">
          <div v-for="(element,index) in arrayInfo" :key="index" class="infoIcons">
              <img v-bind:src="require(`../assets/img/${element.icon}.png`)" :alt="`icona ${element.caption}`">
              <span>{{element.caption}}</span>
          </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'InfoComp',

  data() {
      return {
          arrayInfo: [
            {
                icon: 'buy-comics-digital-comics',
                caption: 'digital comics',
            },

            {
                icon: 'buy-comics-merchandise',
                caption: 'dc merchandise',
            },

            {
                icon: 'buy-comics-subscriptions',
                caption: 'subscription',
            },

            {
                icon: 'buy-comics-shop-locator',
                caption: 'comic shop locator',
            },

            {
                icon: 'buy-dc-power-visa',
                caption: 'dc power visa',
            },
            
          ]
        }
    }

}
</script>

<style scoped lang="scss">
@import '../style/variabili.scss';

.container {
    background-color: $active-blue;
    padding: 30px 0;
    position: relative;
    z-index: 1;

    .row {
        width: 80%;
        margin: 0 auto;
        color: $text-white;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .infoIcons {
            display: flex;
            align-items: center;
            
            img {
                height: 45px;
                margin-right: 10px;
                

            }

            span {
                text-transform: uppercase;
                font-size: 0.9em;
                font-weight: bold;
            }
        }

    }

}

</style>