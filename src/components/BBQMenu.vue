<template>

    <div class='bbqs'>

        <div class='bbq-header'>

            <h2>B.B.Q</h2>


            <div class='bbq-about'>

                <p>Served with sizzling hot stone pot rice & assortment of side dishes</p>

            </div>
        </div>

        <div class='bbqs-items'>

            <bbq-item v-for='BBQ in BBQs' :BBQ='BBQ' class='card'></bbq-item>
        </div>

    </div>

</template>

<script type="text/javascript">
    import BbqItem from './BBQItem.vue';

    export default {

        components: {

            BbqItem

        },

        data() {
            return {
                BBQs: [{
                        name: 'Kalbi',

                        description: 'Korean BBQ beef short ribs with Kalbi sauce',

                        price: 25,

                    },

                    {
                        name: 'Bul-Go-Gi',

                        description: 'Korean BBQ rib-eye marinated in Bulgogi sauce',

                        price: 21,

                    },

                    {
                        name: 'Spicy BBQ Pork',

                        description: 'Korean BBQ pork loin marinated in spicy Bulgogi sauce',

                        price: 21,

                    },

                    {
                        name: 'Chicken BBQ Bul-Go-Gi',

                        description: 'Korean BBQ chicken slices marinated in Bulgogi sauce',

                        price: 21,

                    },

                    {
                        name: 'Spicy Chicken BBQ Bul-Go-Gi',

                        description: 'Korean BBQ chicken slices marinated in spicy Bulgogi sauce',

                        price: 21,

                    },

                ]
            }
        }
    }
</script>

<style type="text/css">
    .bbqs {
        display: grid;
        grid-template-columns: 1fr;
        grid-gap: 20px;
    }

    .bbqs-items {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        grid-gap: 10px;

    }

    .bbq-item-card {
        padding: 15px;
    }

    .bbq-header {
        font-size: 1.5em;

        text-align: center;

        background-color: yellow;
    }

    .bbq-about {
        font-size: .55em;

        line-height: 1;
    }

</style>
