<template>

    <div class='appetizers-item-card'>

        <h3 class='menu-title'>{{appetizer.name}}</h3>

        <p class='appetizers-description'>{{appetizer.description}}</p>

        <span class='price'>${{appetizer.price}}</span>

    </div>

</template>

<script type="text/javascript">

    export default {

        props: ['appetizer']

    }

</script>

<style type="text/css">
    .appetizers-description {
        line-height: 1;
        font-size: .7em;
    }

</style>
