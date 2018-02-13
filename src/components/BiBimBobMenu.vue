<template>

    <div class='bibimbobs'>

        <div class='bibimbob-header'>

            <h2>Bi-Bim-Bobs</h2>

            <div class='bibimbob-about'>
                <p> Served with rice and assortment of side dishes.</p>

                <p><i class='fa fa-leaf'></i> The following can be made into vegetarian dish upon request.</p>
            </div>
        </div>


        <div class='bibimbobs-items'>

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

    .bibimbobs {
        display: grid;
        grid-template-columns: 1fr;
        grid-gap: 20px;
    }

    .bibimbobs-items  {
        display: grid;
        grid-gap: 10px;
        grid-template-columns: repeat(auto-fill, minmax(300px,1fr));
    }

    .bibimbob-item-card {
        padding: 10px;
    }

    .bibimbob-header {
        text-align: center;

        font-size: 1.5em;

        background-color: yellow
     }

    .bibimbob-about {
        font-size: .55em;

        line-height: 1;

    }

</style>
