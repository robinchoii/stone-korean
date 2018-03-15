<template>
    <div class='gallery'>
        <food-picture v-for='image in images' :image='image' :key='image.id' class='food-container'></food-picture>
    </div>
</template>

<script>
    import FoodPicture from './FoodPicture.vue'

    export default {

      name: 'ImageGallery',

      components: {
        FoodPicture
      },

      data () {
        return {
            images: [
            {
                id: 23,
                path: '/assets/stone23.jpg'
            },
            {
                id: 11,
                path: '/assets/stone11.jpg'
            },
            {
                id: 12,
                path: '/assets/stone12.jpg'
            },
            {
                id: 6,
                path: '/assets/stone6.jpg'
            },
            {
                id: 16,
                path: '/assets/stone16.jpg'
            },
            {
                id: 17,
                path: '/assets/stone17.jpg'
            },
            {
                id: 7,
                path: '/assets/stone7.jpg'
            },
            {
                id: 2,
                path: '/assets/stone2.jpg'
            },
            {
                id: 13,
                path: '/assets/stone13.jpg'
            },
            {
                id: 15,
                path: '/assets/stone15.jpg'
            },
            {
                id: 10,
                path: '/assets/stone10.jpg'
            },
            {
                id: 3,
                path: '/assets/stone3.jpg'
            },
            {
                id: 20,
                path: '/assets/stone20.jpg'
            },
            {
                id: 14,
                path: '/assets/stone14.jpg'
            },
            {
                id: 4,
                path: '/assets/stone4.jpg'
            },
            {
                id: 9,
                path: '/assets/stone9.jpg'
            },

            {
                id: 1,
                path: '/assets/stone1.jpg'
            },
            {
                id: 18,
                path: '/assets/stone18.jpg'
            },
            {
                id: 5,
                path: '/assets/stone5.jpg'
            },
            {
                id: 19,
                path: '/assets/stone19.jpg'
            }]
        }
      }
    }
</script>

<style lang="css" scoped>
    .gallery {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        justify-items: center;
        grid-row-gap: 20px;

    }
</style>
