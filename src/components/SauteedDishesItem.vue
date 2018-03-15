<template>

    <div class='sauteed-item-card item-card'>

        <h3 class='item-title'>{{sauteed.name}} <i v-show='sauteed.isVege' class='fa fa-leaf'></i></h3>

        <span class='item-price'>${{sauteed.price}}</span>

        <p class='item-description'>{{sauteed.description}}</p>

    </div>

</template>

<script type="text/javascript">

    export default {
        props: ['sauteed']
    }

</script>
