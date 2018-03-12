<template>

    <div class='appetizers-item-card item-card'>

        <h3 class='item-title'>{{appetizer.name}}</h3>

        <span class='item-price'>{{appetizer.price}}</span>

        <p class='item-description'>{{appetizer.description}}</p>

    </div>

</template>

<script type="text/javascript">

    export default {

        props: ['appetizer']

    }

</script>

<style type="text/css">

</style>
