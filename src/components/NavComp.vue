<template>
  <div>
      <ul>
          <li>characters</li>
          <li class="active">comics</li>
          <li>movies</li>
          <li>tv</li>
          <li>games</li>
          <li>collectibles</li>
          <li>videos</li>
          <li>fans</li>
          <li>news</li>
          <li>shop</li>
      </ul>
  </div>
</template>

<script>
export default {
  name: 'NavComp',

}
</script>

<style scoped lang="scss">

@import '../style/variabili.scss';

ul {
    list-style-type: none;
    display: flex;

    li {
        text-transform: uppercase;
        font-weight: bold;
        font-size: 0.9em;
        padding: 20px 0;
        margin: 0 15px;
        
        &:hover {
            cursor: pointer;
            opacity: 0.6;
        }
    }


    li:not(.active){
        border-bottom: 3px solid transparent;
    }

    li.active {
        color: $active-blue;
        border-bottom: 3px solid $active-blue;
    }
}

</style>