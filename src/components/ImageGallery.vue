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
            // {
            //     id: 1,
            //     path: '/src/assets/stone-pic1.jpg',
            // },
            {
                id: 16,
                path: '/src/assets/stone-pic16.jpg',
            },
            {
                id: 14,
                path: '/src/assets/stone-pic14.jpg',
            },
            {
                id: 15,
                path: '/src/assets/stone-pic15.jpg',
            },
            {
                id: 11,
                path: '/src/assets/stone-pic11.jpg',
            },
            {
                id: 3,
                path: '/src/assets/stone-pic3.jpg',
            },
            {
                id: 5,
                path: '/src/assets/stone-pic5.jpg',
            },
            {
                id: 6,
                path: '/src/assets/stone-pic6.jpg',
            },
            {
                id: 17,
                path: '/src/assets/stone-pic17.jpg',
            },
            {
                id: 2,
                path: '/src/assets/stone-pic2.jpg',
            },
            // {
            //     id: 7,
            //     path: '/src/assets/stone-pic7.jpg',
            // },
            // {
            //     id: 8,
            //     path: '/src/assets/stone-pic8.jpg',
            // },
            {
                id: 12,
                path: '/src/assets/stone-pic12.jpg',
            },
            {
                id: 9,
                path: '/src/assets/stone-pic9.jpg',
            },
            {
                id: 13,
                path: '/src/assets/stone-pic13.jpg',
            },
            {
                id: 10,
                path: '/src/assets/stone-pic10.jpg',
            },
            {
                id: 4,
                path: '/src/assets/stone-pic4.jpg',
            },

            ]
        }
      }
    }
</script>

<style lang="css" scoped>
    .gallery {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
        justify-items: center;
        grid-row-gap: 20px;

    }
</style>
