<template>
    <div class='columns is-mobile'>

        <div class='softTofuSoup column'>

            <div class='softTofuSoup-header '>

                <h2>Soft Tofu Soups</h2>

                <div class='softTofuSoup-about'>
                    <p>Served with sizzling stone pot rice and assortment of side dishes</p>
                    <p>Soft tofu sou can be prepared from non-spicy to extra spicy (5 star scale) according to your preference. </p>
                </div>

            </div>

            <div class='softTofuSoup-flex-grid'>

                <soft-tofu-soup-item v-for='softTofuSoup in softTofuSoups'  class='card' :softTofuSoup="softTofuSoup"></soft-tofu-soup-item>

            </div>

        </div>

    </div>

</template>

<script type="text/javascript">

    import SoftTofuSoupItem from './SoftTofuSoupItem.vue';

    export default {

        components: { SoftTofuSoupItem },

        data() {

            return {
                softTofuSoups: [{
                        name: 'Mushroom Tofu Soup',

                        price: 12

                    },

                    {
                        name: 'Combo Tofu Soup',

                        price: 12

                    },

                    {
                        name: 'Seafood Tofu Soup',

                        price: 12

                    },

                    {
                        name: 'Kimchi Tofu Soup',

                        price: 12

                    },

                    {
                        name: 'Kimchi Beef Tofu Soup',

                        price: 12

                    },

                    {
                        name: 'Kimchi Pork Tofu Soup',

                        price: 12

                    },

                    {
                        name: 'Fish Roe Tofu Soup',

                        price: 12

                    },

                    {
                        name: 'Beef Tofu Soup',

                        price: 12

                    },

                    {
                        name: 'Pork Tofu Soup',

                        price: 12

                    },

                    {
                        name: 'Dumpling Tofu Soup',

                        price: 12

                    },

                    {
                        name: 'Vegetable Tofu Soup',

                        price: 12

                    },

                ]

            }

        }

    }

</script>

<style type="text/css">

    .softTofuSoup-flex-grid {
        display: grid;

        grid-template-columns: 33% 33% 33%;

        grid-template-rows: 33% 33% 33%;

    }

    .softTofuSoup-item-card {
        margin: 5px;

        text-align: center;

        padding: 15px;

    }

    .softTofuSoup-header{
        text-align: center;

        font-size: 1.5em;

        background-color: yellow
     }

    .softTofuSoup-about {
        text-align: center;

        font-size: .6em;

        line-height: 1;

    }

</style>
