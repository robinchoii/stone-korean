<template>

    <div class='bbq-item-card'>

        <h3 class='item-title'>{{BBQ.name}}</h3>

        <p class='item-description'>{{BBQ.description}}</p>

        <span class='item-price'>${{BBQ.price}}</span>

    </div>

</template>


<script type="text/javascript">

    export default  {

        props: ['BBQ']

    }

</script>

<style type="text/css">


</style>
