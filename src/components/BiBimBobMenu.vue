<template>

    <div class='bibimbobs food-wrapper'>

        <div class='bibimbob-header main-header'>

            <h2>Bi-Bim-Bobs</h2>

            <div class='bibimbob-about main-about'>
                <p> Served with rice and side dishes</p>

                <p><i class='fa fa-leaf vege'></i> Ask for Vegetarian</p>
            </div>
        </div>


        <div class='bibimbobs-items food-items-grid'>

            <bi-bim-bob-item v-for='bibimbob in Bibimbobs' :key='bibimbob.id' :bibimbob='bibimbob' class='card'></bi-bim-bob-item>

        </div>

    </div>

</template>

<script type="text/javascript">
    import BiBimBobItem from './BiBimBobItem.vue';

    export default {

        components: {

            BiBimBobItem

        },

        data() {
            return {
                Bibimbobs: [{
                        id: 1,
                        name: 'Beef Hot Pot',
                        description: 'Beef, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '16'
                    },

                    {
                        id: 2,
                        name: 'Seafood Hot Pot',
                        description: 'Seafood, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '16'
                    },

                    {
                        id: 3,
                        name: 'Pork Hot Pot',
                        description: 'Pork, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '16'
                    },

                    {
                        id: 4,
                        name: 'Chicken Hot Pot',
                        description: 'Chicken, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '16'
                    },

                    {
                        id: 5,
                        name: 'Tofu Hot Pot',
                        description: 'Tofu, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '16'
                    },

                    {
                        id: 6,
                        name: 'Vegetable Hot Pot',
                        description: 'Carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '16',
                        isVege: true,

                    },

                    {
                        id: 7,
                        name: 'Cold Bi-Bim-Bob',
                        description: 'Beef, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '13'

                    },
                ]
            }
        }
    }


</script>

<style type="text/css">

</style>
