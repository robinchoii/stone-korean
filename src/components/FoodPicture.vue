<template>
    <div class="image-container'">
        <div class='image'>
            <img :src="image.path" alt='image.alt'/><br>
        </div>
        <span>{{image.alt}}</span>
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
        width: 298px;
        height: 175px;
        object-fit: cover;

    }
    .image {
        border: 1px solid white;
     }


</style>
