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
        width: 293px;
     }
     .logo-image {
        background-image: url('/src/assets/stone-logo.png');
        background-repeat: no-repeat;
        height: 78px;
        width: 293px;
        margin:0;
     }
     .logo-image:hover {
        cursor: pointer
     }
</style>
