<template>

    <div class='fried-chicken-item-card'>

        <h3 class='item-title'>{{chicken.name}}</h3>

        <p class='item-description'>{{chicken.description}}</p>

        <span class='item-price'>${{chicken.price}}</span>

    </div>

</template>

<script type="text/javascript">

    export default  {
        props: ['chicken']
    }

</script>

<style type="text/css"></style>
