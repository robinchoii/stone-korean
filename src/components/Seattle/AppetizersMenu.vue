<template>
    <div class='appetizers food-wrapper'>

        <div class='appetizers-header main-header'>

            <h2>Appetizers</h2>

            <div class='appetizers-about main-about'>

                <p><i class='fa fa-leaf'></i> Ask for Vegetarian</p>

            </div>

        </div>

        <div class='appetizer-items food-items-grid'>

            <appetizers-item v-for='appetizer in appetizers' :key='appetizer.id'  class='card' :appetizer='appetizer'></appetizers-item>

        </div>

    </div>

</template>

<script type="text/javascript">

    import AppetizersItem from './AppetizerItem.vue';

    export default {

        components: { AppetizersItem },

        data() {

            return {
                appetizers: [{

                    id: 1,

                        name: 'Gyoza, 10pcs',

                        description: "Pork & vegetable potstickers, served with soy dipping sauce",

                        price: 8,

                        isVege: false,

                    },

                    {
                        id: 2,

                        name: 'Seafood Pancake',

                        description: "Pan-fried seafood (baby shrimp, baby octopus & calamari squid) pancake with green onions, served with soy dipping sauce",

                        price: 17

                    },

                    {
                        id: 3,

                        name: 'Kimchi Pancake',

                        description: "Pan-fried Kimchi pancake with soy dipping sauce",

                        price: 15,

                        isVege: true,

                    },

                    {
                        id: 4,

                        name: 'Veggie Pancake',

                        description: "Pan-fried veggies(green and white onions, carrot, & bellpepper) pancake with soy dipping sauce",

                        price: 15,

                        isVege: true,
                    },

                    {
                        id: 5,

                        name: 'Steamed Egg',

                        description: "Battered egg, steamed with chopped green onions",

                        price: 8,

                        isVege: false,

                    },

                    {
                        id: 6,

                        name: 'Jab-Chae',

                        description: "Korean potato starch noodles, stir-fried with veggies & beef, seasoned in soy sauce",

                        price: 15,

                        isVege: true,

                    },

                    {
                        id: 7,

                        name: 'Dduhk-Bohk-Ghi',

                        description: "Fresh rice cake & veggies, boiled & braised in sweet Korean chili sauce",

                        price: 12,

                        isVege: true,

                    },

                    {
                        id: 8,

                        name: 'Chicken Hot Wings, 8pcs',

                        description: "Seasoned chicken wings deep-fried in soybean oil",

                        price: 13

                    }
                ],

            }

        }

    }

</script>

<style type="text/css">

</style>
