<template>

    <div class='bibimbobs food-wrapper'>

        <div class='bibimbob-header main-header'>

            <h2>Bi-Bim-Bobs</h2>

            <div class='bibimbob-about main-about'>
                <p> Served with rice and assortment of side dishes.</p>

                <p><i class='fa fa-leaf vege'></i> The following can be made into vegetarian dish upon request.</p>
            </div>
        </div>


        <div class='bibimbobs-items food-items-grid'>

            <bi-bim-bob-item v-for='bibimbob in Bibimbobs' :bibimbob='bibimbob' class='card'></bi-bim-bob-item>

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

                        name: 'Beef Hot Pot Bi-Bim-Bob',
                        description: 'Beef, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '15'

                    },

                    {

                        name: 'Seafood Hot Pot Bi-Bim-Bob',
                        description: 'Seafood, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '15'

                    },

                    {

                        name: 'Pork Hot Pot Bi-Bim-Bob',
                        description: 'Pork, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '15'
                    },

                    {

                        name: 'Chicken Hot Pot Bi-Bim-Bob',
                        description: 'Chicken, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '15'

                    },

                    {

                        name: 'Tofu Hot Pot Bi-Bim-Bob',
                        description: 'Tofu, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '14'

                    },

                    {

                        name: 'Kimchi Hot Pot Bi-Bim-Bob',
                        description: 'Well-ripen Kimchi, carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '14'

                    },

                    {

                        name: 'Vegetable Hot Pot Bi-Bim-Bob',
                        description: 'Carrots, shiitake mushrooms, zucchini, bean-sprouts, spinach. Topped with yolk of an egg. Served in a sizzling hot stone pot.',
                        price: '14'

                    },

                    {

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
