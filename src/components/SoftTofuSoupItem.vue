<template>

    <div class='softTofuSoup-item-card'>

        <h3 class='item-title'>{{softTofuSoup.name}}</h3>

        <span class='item-price'>${{softTofuSoup.price}}</span>

    </div>

</template>

<script type="text/javascript">

    export default {

        props: ['softTofuSoup']

    }

</script>

<style type="text/css">

</style>
