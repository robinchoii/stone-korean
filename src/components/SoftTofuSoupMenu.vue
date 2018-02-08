<template>
    <div class='soft-tofu-soups'>

        <div class='soft-tofu-soups-header'>

            <h2>Soft Tofu Soups</h2>

            <div class='soft-tofu-soups-about'>
                <p>Served with sizzling stone pot rice and assortment of side dishes</p>
                <p>Soft tofu sou can be prepared from non-spicy to extra spicy (5 star scale) according to your preference. </p>
                <p><i class='fa fa-leaf'></i> The following can be made into vegetarian dish upon request.</p>
            </div>

        </div>

        <div class='soft-tofu-soups-items'>

            <soft-tofu-soup-item v-for='softTofuSoup in softTofuSoups'  class='card' :softTofuSoup="softTofuSoup"></soft-tofu-soup-item>

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
    .soft-tofu-soups {
        display: grid;
        grid-template-columns: 1fr;
        grid-gap: 20px;
    }

    .soft-tofu-soups-items {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
        grid-gap: 10px;
        text-align: center;
    }


    .soft-tofu-soups-header{
        text-align: center;
        font-size: 1.5em;
        background-color: yellow
     }

    .soft-tofu-soups-about {
        font-size: .55em;
        line-height: 1;

    }

</style>
