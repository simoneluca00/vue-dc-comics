<template>
    <div class="series">
        <img :src="thumb" :alt="'copertina di ' + series">
        <h5>{{series}}</h5>
    </div>
</template>

<script>
    export default {
        name: 'ProductComp',

        props: {
            thumb: String,
            series: String,
        }

    }
</script>

<style scoped lang="scss">

    .series {
        flex-basis: calc(100% / 6);
        margin-bottom: 40px;

        h5 {
         text-transform: uppercase;
        }

    }

</style>