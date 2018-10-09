<template>

    <div class='fried-chicken-item-card item-card'>

        <h3 class='item-title'>{{chicken.name}}</h3>

        <span class='item-price'>${{chicken.price}}</span>

        <p class='item-description'>{{chicken.description}}</p>

    </div>

</template>

<script type="text/javascript">

    export default  {
        props: ['chicken']
    }

</script>

<style type="text/css"></style>
