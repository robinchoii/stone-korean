<template>

    <div class='sauteed-dishes food-wrapper'>

        <div class='sauteed-dishes-header main-header'>

            <h2>Sauteed Dishes</h2>

            <div class='sauteed-dishes-about main-about'>

                <p>Served with a sizzling hot stone pot rice and side dishes</p>

                <p><i class='fa fa-leaf'></i> Vegetarian upon request</p>

            </div>

        </div>

        <div class='sauteed-dishes-items food-items-grid'>

            <sauteed-dishes-item v-for='sauteed in sauteedDishes' :key='sauteed.id' :sauteed='sauteed' class='card'></sauteed-dishes-item>

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
                        id: 1,
                        name:'Spicy Squid',
                        description: 'Sauteed squid & vegetables with house spicy sauce',
                        price: 19,
                    },
                    {
                        id: 2,
                        name:'Shrimp Stir Fried Vegetables',
                        description: 'Sauteed shrimp & vegetables with house sauce',
                        price: 17,
                    },
                    {
                        id: 3,
                        name:'Chicken Stir Fried Vegetables',
                        description: 'Sauteed chicken & vegetables with house sauce',
                        price: 16,
                    },
                    {
                        id: 4,
                        name:'Stif Fried Vegetables',
                        description: 'Sauteed vegetables with house sauce',
                        price: 15,
                        isVege: true,
                    }
                ]
            }
        }
    }
</script>

<style type="text/css">

</style>
