<template>

    <div class='lunch-item-card'>

        <h3 class='menu-title'>{{lunch.name}}</h3>

        <p class='lunch-description'>{{lunch.description}}</p>

        <span class='price'>${{lunch.price}}</span>

    </div>

</template>

<script type="text/javascript">

    export default {

        props: ['lunch']

    }

</script>

<style type="text/css">

    .lunch-description {
        line-height: 1;
        font-size: .7em;
    }

</style>
