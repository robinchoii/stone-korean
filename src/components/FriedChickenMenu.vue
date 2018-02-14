<template>

    <div class='fried-chicken'>

        <div class='fried-chicken-header'>
            <h2>Fried Chicken</h2>
            <div class='fried-chicken-about'>
                <p>Deep fried in soy bean oil. </p>
                <p>Served with side of pickled radishes. Must pair with entre for full side dish set.</p>
            </div>
        </div>

        <div class='fried-chicken-items'>

            <fried-chicken-item v-for='chicken in chickens' :chicken='chicken' class='card'></fried-chicken-item>

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
                        name:'Fried Chicken',
                        description: 'Whole fried chicken cut into 12 pieces with house made batter',
                        price: 22,
                    },
                    {
                        name:'Marinated Chicken',
                        description: 'Whole fried chicken cut into 12 pieces toss in a sweet garlic sauce',
                        price: 23,
                    },
                    {
                        name:'1/2 Fried 1/2 Marinated',
                        description: 'Whole fried chicken cut into 12 pieces, half fried and half marinated',
                        price:25,
                    },
                    {
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

    .fried-chicken {
        display: grid;
        grid-gap: 20px;
        grid-template-columns: 1fr;

    }

    .fried-chicken-items {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        grid-gap: 10px;
    }

    .fried-chicken-item-card {
        padding: 10px;
    }

    .fried-chicken-header {
        font-size: 1.5em;
        text-align: center;
        background-color: yellow;

    }

    .fried-chicken-about {
        font-size: .55em;
        line-height: 1;

    }
</style>
