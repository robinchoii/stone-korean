<template>

    <div class='lunch-item columns'>

        <div class='column'>

            <h3>{{lunch.name}}</h3>

            <p class='description'>{{lunch.description}}</p>


        </div>

        <div class='column'>

            <span>{{lunch.price}}</span>

        </div>
    </div>

</template>

<script type="text/javascript">

    export default {

        props: ['lunch']

    }

</script>

<style type="text/css">

    .description {
        line-height: .5;
        font-size:.75em;

    }

</style>
