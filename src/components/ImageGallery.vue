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
            images: [{
                id: 1,
                path: '/stone1.jpg'
            },
            {
                id: 2,
                path: '/stone2.jpg'
            },
            {
                id: 3,
                path: '/stone3.jpg'
            },
            {
                id: 4,
                path: '/stone4.jpg'
            },
            {
                id: 5,
                path: '/stone5.jpg'
            },
            {
                id: 6,
                path: '/stone6.jpg'
            },
            {
                id: 7,
                path: '/stone7.jpg'
            },
            {
                id: 8,
                path: '/stone8.jpg'
            },
            {
                id: 9,
                path: '/stone9.jpg'
            },
            {
                id: 10,
                path: '/stone10.jpg'
            },
            {
                id: 11,
                path: '/stone11.jpg'
            },
            {
                id: 12,
                path: '/stone12.jpg'
            },
            {
                id: 13,
                path: '/stone13.jpg'
            },
            {
                id: 14,
                path: '/stone14.jpg'
            },
            {
                id: 15,
                path: '/stone15.jpg'
            },
            {
                id: 16,
                path: '/stone16.jpg'
            },
            {
                id: 17,
                path: '/stone17.jpg'
            },
            {
                id: 18,
                path: '/stone18.jpg'
            },
            {
                id: 19,
                path: '/stone19.jpg'
            },
            {
                id: 20,
                path: '/stone20.jpg'
            },
            // {
            //     id: 21,
            //     path: '/stone21.jpg'
            // },
            // {
            //     id: 22,
            //     path: '/stone22.jpg'
            // },
            {
                id: 23,
                path: '/stone23.jpg'
            }]
        }
      }
    }
</script>

<style lang="css" scoped>
    .gallery {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    }
</style>
