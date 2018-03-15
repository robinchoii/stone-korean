<template>
    <div class='soft-tofu-soups food-wrapper'>

        <div class='soft-tofu-soups-header main-header'>

            <h2>Soft Tofu Soups</h2>

            <div class='soft-tofu-soups-about main-about'>

                <p>Served with sizzling stone pot rice and assortment of side dishes</p>

                <p>Soft tofu sou can be prepared from non-spicy to extra spicy (5 star scale) according to your preference. </p>

                <p><i class='fa fa-leaf'></i> The following can be made into vegetarian dish upon request.</p>

            </div>

        </div>

        <div class='soft-tofu-soups-items food-items-grid'>

            <soft-tofu-soup-item v-for='softTofuSoup in softTofuSoups' :key='softTofuSoup.id' class='card' :softTofuSoup="softTofuSoup"></soft-tofu-soup-item>

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
                        id: 1,

                        name: 'Mushroom Tofu Soup',

                        price: 12,

                        isVege: true,

                    },

                    {
                        id: 2,

                        name: 'Combo Tofu Soup',

                        price: 12

                    },

                    {
                        id: 3,

                        name: 'Seafood Tofu Soup',

                        price: 12

                    },

                    {
                        id: 4,

                        name: 'Kimchi Tofu Soup',

                        price: 12,

                        isVege: true,

                    },

                    {
                        id: 5,

                        name: 'Kimchi Beef Tofu Soup',

                        price: 12

                    },

                    {
                        id: 6,

                        name: 'Kimchi Pork Tofu Soup',

                        price: 12

                    },

                    {
                        id: 7,

                        name: 'Fish Roe Tofu Soup',

                        price: 12

                    },

                    {
                        id: 8,

                        name: 'Beef Tofu Soup',

                        price: 12

                    },

                    {
                        id: 9,

                        name: 'Pork Tofu Soup',

                        price: 12

                    },

                    {
                        id: 10,

                        name: 'Dumpling Tofu Soup',

                        price: 12,

                        isVege: true,

                    },

                    {
                        id: 11,

                        name: 'Vegetable Tofu Soup',

                        price: 12,

                        isVege: true,

                    },

                ]

            }

        }

    }

</script>

<style type="text/css">


</style>
