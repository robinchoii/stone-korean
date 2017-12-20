<template>

    <div class='bbq-item-card'>

        <h3 class='menu-title'>{{BBQ.name}}</h3>

        <p class='bbq-description'>{{BBQ.description}}</p>

        <span class='price'>${{BBQ.price}}</span>

    </div>

</template>


<script type="text/javascript">

    export default  {

        props: ['BBQ']

    }

</script>

<style type="text/css">
    .bbq-description {
        font-size: .7em;
    }

</style>
