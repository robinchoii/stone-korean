<template>

    <div class='columns'>

        <div class='column'>

            <div class='sauteed-header'>
                <h2>Sauteed Dishes Chicken</h2>
                <div class='sauteed-about'>
                    <p>Served with a sizzling hot stone pot rice and assortment of side dishes.</p>
                    <p><i class='fa fa-leaf'></i>The following can be made into vegetarian dish upon request.</p>
                </div>
            </div>

            <div class='sauteed-flex-grid'>

                <sauteed-dishes-item v-for='sauteed in sauteedDishes' :sauteed='sauteed' class='card'></sauteed-dishes-item>

            </div>

        </div>

    </div>

</template>

<script type="text/javascript">
    import SauteedDishesItem from './SauteedDishesItem.vue'

    export default {

        components: {

            SauteedDishesItem

        },

        data() {
            return {
                sauteedDishes: [{
                        name:'Spicy Squid',
                        description: 'Sauteed squid & vegetables with house spicy sauce',
                        price: 15,
                    },
                    {
                        name:'Spicy Squid w/ Noodles',
                        description: 'Sauteed squid & vegetables with Udon noodles with house spicy sauce',
                        price: 18,
                    },
                    {
                        name:'Shrimp Stir Fried Vegetables',
                        description: 'Sauteed shrimp & vegetables with house sauce',
                        price: 16,
                    },
                    {
                        name:'Chicken Stir Fried Vegetables',
                        description: 'Sauteed chicken & vegetables with house sauce',
                        price: 15,
                    },
                    {
                        name:'Stif Fried Vegetables',
                        description: 'Sauteed vegetables with house sauce',
                        price: 13,
                    },
                    {
                        name:'Stif Fried Vegetables w/ Noodles',
                        description: 'Sauteed vegetables & spinach noodles with house sauce',
                        price: 15,
                    }
                ]
            }
        }
    }
</script>

<style type="text/css">

    .sauteed-flex-grid {
        display: grid;

        grid-template-columns: 33% 33% 33%;

        grid-template-rows: 33% 33% 33%;

    }

    .sauteed-item-card {
        margin: 5px;

        text-align: center;

        padding: 15px;
    }

    .sauteed-header {

        font-size: 1.5em;

        text-align: center;

        background-color: yellow;

    }

    .sauteed-about {

        font-size: .6em;

        line-height: 1;

    }
</style>
