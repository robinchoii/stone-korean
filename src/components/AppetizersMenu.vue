<template>
    <div class='columns is-mobile'>

        <div class='appetizers-conatiner column'>

            <div class='appetizers-header'>

                <h2>Appetizers</h2>

            </div>

            <div class='appetizers-flex-grid'>

                <appetizers-item v-for='appetizer in appetizers' class='card' :appetizer='appetizer'></appetizers-item>

            </div>

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
                        name: 'Dumplings, 10pcs.',

                        description: "Pork & vegetable potstickers, served with soy dipping sauce",

                        price: 7

                    },

                    {
                        name: 'Seafood Pancake',

                        description: "Pan-fried seafood (baby shrimp, baby octopus & calamari squid) pancake with green onions, served with soy dipping sauce",

                        price: 15

                    },

                    {
                        name: 'Kimchi Pancake',

                        description: "Pan-fried Kimchi pancake with soy dipping sauce",

                        price: 12

                    },

                    {
                        name: 'Veggie Pancake',

                        description: "Pan-fried veggies(green and white onions, carrot, & bellpepper) pancake with soy dipping sauce",

                        price: 12
                    },

                    {
                        name: 'Gye-Rahn-Jiim',

                        description: "Battered egg, steamed with chopped green onions",

                        price: 7

                    },

                    {
                        name: 'Jab-Chae',

                        description: "Korean potato starch noodles, stir-fried with veggies & beef, seasoned in soy sauce",

                        price: 14

                    },

                    {
                        name: 'Dduhk-Bohk-Ghi',

                        description: "Fresh rice cake & veggies, boiled & braised in sweet Korean chili sauce",

                        price: 10

                    },

                    {
                        name: 'Chicken Hot Wings, 8pcs.',

                        description: "Seasoned chicken wings deep-fried in soybean oil",

                        price: 12

                    },

                ],

            }

        }

    }

</script>

<style type="text/css">

    .appetizers-flex-grid {
        display: grid;

        grid-template-columns: 33% 33% 33%;

        grid-template-rows: 33% 33% 33%;

    }

    .appetizers-item-card {
        margin: 5px;

        text-align: center;

        padding: 15px;

    }

    .appetizers-header{
        text-align: center;

        font-size: 1.5em;

        background-color: yellow
     }

    .appetizers-description {
        font-size: .5em;

        line-height: 1;

    }

</style>
