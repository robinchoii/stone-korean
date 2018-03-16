<template>
    <div class='lunch-specials food-wrapper'>

        <div class='lunch-header main-header'>

            <h2>Lunch Specials</h2>

            <div class='lunch-about main-about'>

                <p>11:00am - 2:30pm, Monday - Friday (Except Holidays)</p>

                <p>Rice and assortment of sides included</p>

                <p><i class='fa fa-leaf'></i> Ask for Vegetarian</p>

            </div>

        </div>

        <div class='lunch-items food-items-grid'>

            <lunch-item v-for='lunch in lunches' :key='lunch.id' class='card' :lunch='lunch'></lunch-item>

        </div>

    </div>

</template>

<script type="text/javascript">
    import LunchItem from './LunchItem.vue';
    import AppetizerItem from './AppetizerItem.vue';

    export default {

        components: { LunchItem, AppetizerItem},

        data() {

            return {
                lunches: [{
                        id: 1,

                        name: "Soft Tofu Soup",

                        description: "Choose one of our Soft Tofu Soups",

                        price: 11,

                        isVege: true,

                    },

                    {
                        id: 2,

                        name: 'Cold Bi-Bim-Bob',

                        description: "Assorted vegetables, beef & egg over rice",

                        price: 10,

                        isVege: true

                    },

                    {
                        id: 3,

                        name: 'Hot Pot Bi-Bim-Bob',

                        description: "Assorted vegetables, beef & egg over rice in a sizzling stone pot",

                        price: 13,

                        isVege: true,

                    },

                    {
                        id: 4,

                        name: 'Bul-Go-Gi',

                        description: "BBQ beef ribeye served with onions topped with sesame seeds",

                        price: 12


                    },

                    {
                        id: 5,

                        name: 'Kalbi',

                        description: "BBQ beef short ribs served with onions topped with sesame seeds",

                        price: 13

                    },

                    {
                        id: 6,

                        name: 'Spicy Pork Bul-Go-Gi',

                        description: "Spicy BBQ pork loin served with onions topped with sesame seeds ",

                        price: 12

                    },

                    {
                        id: 7,

                        name: 'Chicken Bul-Go-Gi',

                        description: "BBQ chicken slices served with onions topped with sesame seeds",

                        price: 12

                    },

                    {
                        id: 8,

                        name: 'Spicy Chicken Bul-Go-Gi',

                        description: "Spicy BBQ chicken slices served with onions topped with sesame seeds",

                        price: 12

                    },

                    {
                        id: 9,

                        name: 'Yuk-Gae-Jahng',

                        description: "Spicy beef brisket and vegetable soup",

                        price: 12

                    },

                    {
                        id: 10,

                        name: 'Kimchi Jhi-Gae',

                        description: "Kimchi stew with onions, medium-firm tofu, rice cakes. Choice of Beef or Pork",

                        price: 10,

                        isVege: true

                    }
                ]

            }

        }

    }

</script>

<style type="text/css">


</style>
