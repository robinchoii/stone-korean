<template>

    <div class='bibimbob-item-card item-card'>
        <h3 class='item-title'>{{bibimbob.name}}</h3>

        <span class='item-price'>${{bibimbob.price}}</span>

        <p class='item-description'>{{bibimbob.description}}</p>
    </div>

</template>

<script type="text/javascript">

    export default {

        props: ['bibimbob']

    }

</script>

<style type="text/css">


</style>
