<template>
    <div>
        <div class="logo-container">
            <a href="/">
                <figure class="logo-image"></figure>
            </a>
        </div>
    </div>

</template>

<script>
    export default {

    }

</script>

<style type="text/css">
     .logo-container {
        margin: 0 auto;
        width: 325px;
     }
     .logo-image {
        background-image: url('/src/assets/stone-logo-2.png');
        background-repeat: no-repeat;
        background-size: 325px 78px;
        height: 78px;
        width: 325px;
        margin:0;
     }
     .logo-image:hover {
        cursor: pointer
     }
</style>
