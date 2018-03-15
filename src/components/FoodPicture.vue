<template>
    <div class='image'>
        <img :src="'/dist'+image.path" />
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
        height: auto;
        /*object-fit: cover;*/
    }
    .image {
        width: 250px;
        line-height: 0;
     }
</style>
