<template>

    <div class='fried-chicken food-wrapper'>

        <div class='fried-chicken-header main-header'>

            <h2>Fried Chicken</h2>

            <div class='fried-chicken-about main-about'>

                <p>Served with side of pickled radishes <br /> Must pair with entre for full side dish set</p>

            </div>

        </div>

        <div class='fried-chicken-items food-items-grid'>

            <fried-chicken-item v-for='chicken in chickens' :key='chicken.id' :chicken='chicken' class='card'></fried-chicken-item>

        </div>

    </div>

</template>

<script type="text/javascript">
    import FriedChickenItem from './FriedChickenItem.vue'

    export default {
        components: {

            FriedChickenItem

        },

        data() {
            return {
                chickens: [{
                        id: 1,
                        name:'Fried Chicken',
                        description: 'Whole fried chicken cut into 12 pieces with house made batter',
                        price: 22,
                    },
                    {
                        id: 2,
                        name:'Marinated Chicken',
                        description: 'Whole fried chicken cut into 12 pieces toss in a sweet garlic sauce',
                        price: 23,
                    },
                    {
                        id: 3,
                        name:'1/2 Fried 1/2 Marinated',
                        description: 'Whole fried chicken cut into 12 pieces, half fried and half marinated',
                        price:25,
                    },
                    {
                        id: 4,
                        name:'Chicken Hot Wings',
                        description: 'Fried hot wings, 12 pieces',
                        price: 17,
                    },
                    {
                        name:'Chili Marinated Hot Wings',
                        description: 'Fried Hot wings tossed in a spicy, sweet garlic sauce',
                        price: 18,
                    }
                ]
            }
        }
    }
</script>

<style type="text/css">


</style>
