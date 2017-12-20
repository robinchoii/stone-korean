<template>

    <div class='sauteed-item-card'>

        <h3 class='item-title'>{{sauteed.name}}</h3>

        <p class='item-description'>{{sauteed.description}}</p>

        <span class='item-price'>${{sauteed.price}}</span>

    </div>

</template>

<script type="text/javascript">

    export default {
        props: ['sauteed']
    }

</script>
