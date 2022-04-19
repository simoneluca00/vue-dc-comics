<template>
    <div class="series">
        <div class="imgSeries">
            <img :src="thumb" :alt="'copertina di ' + series">
        </div>
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

div.products {
    display: flex;
    flex-wrap: wrap;

    .series {
        flex-basis: calc(100% / 6);
        margin-bottom: 40px;

        h5 {
         text-transform: uppercase;
        }

    }
}

</style>