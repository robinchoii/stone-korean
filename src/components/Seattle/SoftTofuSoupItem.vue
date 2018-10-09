<template>

    <div class='soft-tofu-soups-item-card item-card'>

        <h3 class='item-title'>{{softTofuSoup.name}} <i v-show='softTofuSoup.isVege' class='fa fa-leaf'></i></h3>

        <span class='item-price'>${{softTofuSoup.price}}</span>

    </div>

</template>

<script type="text/javascript">

    export default {

        props: ['softTofuSoup']

    }

</script>

<style type="text/css">
    .soft-tofu-soups-item-card {
        padding: 10px;

    }
</style>
