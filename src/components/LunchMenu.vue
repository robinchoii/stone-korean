<template>

    <div class='container'>

        <div class='lunch-header'>

            <h2>Lunch Specials</h2>

        </div>

        <div class='lunch-description'>

            <p>11:00am - 2:30pm, Monday - Friday (Except Holidays)</p>

            <p>Rice and assortment of sides included.</p>

            <p>Bi-Bim-Bob can be made into vegetarian dish upon request.</p>

        </div>

        <div class='lunch-menu'>
            <lunch-item v-for='lunch in lunches' :lunch='lunch'></lunch-item>
        </div>

    </div>

</template>

<script type="text/javascript">
    import LunchItem from './LunchItem.vue';

    export default {

        // props: ['lunches'],

        components: { LunchItem },

        data() {

            return {
                lunches: [{

                        name: "Soft Tofu Soup",

                        description: "Choose one of our Soft Tofu Soups",

                        price: 11,

                    },

                    {

                        name: 'Cold Bi-Bim-Bob',

                        description: "Assorted vegetables, beef & egg over rice",

                        price: 10

                    },

                    {

                        name: 'Hot Pot Bi-Bim-Bob',

                        description: "Assorted vegetables, beef & egg over rice in a sizzling stone pot",

                        price: 13

                    },

                    {

                        name: 'Bul-Go-Gi',

                        description: "BBQ beef ribeye served with onions topped with sesame seeds",

                        price: 12

                    },

                    {

                        name: 'Kalbi',

                        description: "BBQ beef short ribs served with onions topped with sesame seeds",

                        price: 13

                    },

                    {

                        name: 'Spicy Pork Bul-Go-Gi',

                        description: "Spicy BBQ pork loin served with onions topped with sesame seeds ",

                        price: 12

                    },

                    {

                        name: 'Chicken Bul-Go-Gi',

                        description: "BBQ chicken slices served with onions topped with sesame seeds",

                        price: 12

                    },

                    {

                        name: 'Spicy Chicken Bul-Go-Gi',

                        description: "Spicy BBQ chicken slices served with onions topped with sesame seeds",

                        price: 12

                    },

                    {

                        name: 'Yuk-Gae-Jahng',

                        description: "Spicy beef brisket and vegetable soup",

                        price: 12

                    },

                    {

                        name: 'Kimchi Jhi-Gae',

                        description: "Kimchi stew with onions, medium-firm tofu, rice cakes. Choice of Beef or Pork",

                        price: 10

                    }
                ]


            }
        }
    }

</script>

<style type="text/css">

    .lunch-header {

        font-size: 1.5em

     }

    .lunch-description {

        font-size: 1em;
        line-height: 1

    }

    .lunch-menu {

        padding-top: 15px;
    }
</style>
