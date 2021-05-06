<template>

    <div class='bbqs food-wrapper'>

        <div class='bbq-header main-header'>

            <h2>B.B.Q</h2>


            <div class='bbq-about main-about'>

                <p>Served with sizzling hot stone pot rice and side dishes</p>

            </div>
        </div>

        <div class='bbqs-items food-items-grid'>

            <bbq-item v-for='BBQ in BBQs' :key='BBQ.id':BBQ='BBQ' class='card'></bbq-item>
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
                        id: 1,

                        name: 'Kalbi',

                        description: 'Korean BBQ beef short ribs with Kalbi sauce',

                        price: 29,

                    },

                    {
                        id: 2,

                        name: 'Bulgogi',

                        description: 'Korean BBQ rib-eye marinated in Bulgogi sauce',

                        price: 27,

                    },

                    {
                        id: 3,

                        name: 'Spicy Pork Bulgogi',

                        description: 'Korean BBQ pork loin marinated in spicy Bulgogi sauce',

                        price: 27,

                    },

                    {
                        id: 4,

                        name: 'Chicken Bulgogi',

                        description: 'Korean BBQ chicken slices marinated in Bulgogi sauce',

                        price: 27,

                    },

                    {
                        id: 5,

                        name: 'Spicy Chicken Bulgogi',

                        description: 'Korean BBQ chicken slices marinated in spicy Bulgogi sauce',

                        price: 27,

                    },

                ]
            }
        }
    }
</script>

<style type="text/css">

</style>
