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
                alt: 'Seafood Pancake'
            },
            {
                id: 14,
                path: '/src/assets/stone-pic14.jpg',
                alt: 'Spicy Rice Cake'
            },
            {
                id: 15,
                path: '/src/assets/stone-pic15.jpg',
                alt: 'Jabchae'
            },
            {
                id: 11,
                path: '/src/assets/stone-pic11.jpg',
                alt: 'Soft Tofu Soup'
            },
            {
                id: 3,
                path: '/src/assets/stone-pic3.jpg',
                alt: 'Hot Wings'
            },
            {
                id: 5,
                path: '/src/assets/stone-pic5.jpg',
                alt: 'Marinated Chicken'
            },
            {
                id: 6,
                path: '/src/assets/stone-pic6.jpg',
                alt: 'Fried Chicken'
            },
            {
                id: 17,
                path: '/src/assets/stone-pic17.jpg',
                alt: 'Spicy Beef Brisket Soup'
            },
            {
                id: 2,
                path: '/src/assets/stone-pic2.jpg',
                alt: 'Kalbi'
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
                alt: 'Bulgogi'
            },
            {
                id: 9,
                path: '/src/assets/stone-pic9.jpg',
                alt: 'Hot Pot Bibimbob'
            },
            {
                id: 13,
                path: '/src/assets/stone-pic13.jpg',
                alt: 'Cold Bibimbob'
            },
            {
                id: 10,
                path: '/src/assets/stone-pic10.jpg',
                alt: 'Seafood Noodle Soup'
            },
            {
                id: 4,
                path: '/src/assets/stone-pic4.jpg',
                alt: 'Cold Noodle Soup'
            },
            {
                id: 20,
                path: '/src/assets/stone-pic20.jpg',
                alt: 'Side Dishes'
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

    }
</style>
