<template>

    <div class='bibimbob-item-card'>
        <h3 class='menu-title'>{{bibimbob.name}}</h3>

        <p class='bibimbob-description'>{{bibimbob.description}}</p>

        <span class='price'>${{bibimbob.price}}</span>
    </div>

</template>

<script type="text/javascript">

    export default {

        props: ['bibimbob']

    }

</script>

<style type="text/css">

    .bibimbob-description {
        font-size: .7em;
    }
</style>
