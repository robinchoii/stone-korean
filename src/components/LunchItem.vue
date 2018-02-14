<template>

    <div class='lunch-item-card item-card'>

        <h3 class='item-title'>{{lunch.name}}</h3>

        <p class='item-description'>{{lunch.description}}</p>

        <span class='item-price'>${{lunch.price}}</span>

    </div>

</template>

<script type="text/javascript">

    export default {

        props: ['lunch']

    }

</script>

<style type="text/css">

    .lunch-item-card {
        padding: 10px;
    }
</style>
