<template>

    <div class='sauteed-dishes'>

        <div class='sauteed-dishes-header'>
            <h2>Sauteed Dishes</h2>
            <div class='sauteed-dishes-about'>
                <p>Served with a sizzling hot stone pot rice and assortment of side dishes.</p>
                <p><i class='fa fa-leaf'></i>The following can be made into vegetarian dish upon request.</p>
            </div>
        </div>

        <div class='sauteed-dishes-items'>

            <sauteed-dishes-item v-for='sauteed in sauteedDishes' :sauteed='sauteed' class='card'></sauteed-dishes-item>

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

    .sauteed-dishes {
        display: grid;
        grid-template-columns: 1fr;
        grid-gap: 20px;

    }

    .sauteed-dishes-items {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        grid-gap: 10px;
    }

    .sauteed-item-card {
        padding: 10px;
    }

    .sauteed-dishes-header {

        font-size: 1.5em;

        text-align: center;

        background-color: yellow;

    }

    .sauteed-dishes-about {

        font-size: .55em;

        line-height: 1;

    }
</style>
