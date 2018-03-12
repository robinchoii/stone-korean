<template>

    <div class='bbq-item-card item-card'>

        <h3 class='item-title'>{{BBQ.name}}</h3>

        <span class='item-price'>{{BBQ.price}}</span>

        <p class='item-description'>{{BBQ.description}}</p>

    </div>

</template>


<script type="text/javascript">

    export default  {

        props: ['BBQ']

    }

</script>

<style type="text/css">


</style>
