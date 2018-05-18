<template>
    <div class='image'>
        <img :src="image.path" alt='image.alt'/>
    </div>
</template>

<script type="text/javascript">
    export default {
        props: {
            image: {required: true}
        }
    }
</script>

<style type="text/css">
    .image img {
        width: 100%;
        height: 100%;
        object-fit: cover;

    }
    .image {
        // align-self: center;
        // width: 250px;
        // height: auto;
        border: 1px solid white;
     }
</style>
