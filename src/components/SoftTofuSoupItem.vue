<template>

    <div class='softTofuSoup-item-card'>

        <h3 class='menu-title'>{{softTofuSoup.name}}</h3>

        <span class='price'>${{softTofuSoup.price}}</span>

    </div>

</template>

<script type="text/javascript">

    export default {

        props: ['softTofuSoup']

    }

</script>

<style type="text/css">

    .softTofuSoup-description {
        line-height: 1;
        font-size: .7em;
    }

</style>
