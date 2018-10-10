 <template>
    <div class='soft-tofu-soups food-wrapper'>

        <div class='soft-tofu-soups-header main-header'>

            <h2>Soft Tofu Soups</h2>

            <div class='soft-tofu-soups-about main-about'>

                <p>Served with steamed rice and side dishes</p>

                <p><i class='fa fa-leaf'></i> Ask for Vegetarian</p>

                <div class='spicy'>

                    <div class='non-spicy'>
                        <i class="fa fa-star"></i>
                        <div>White</div>
                    </div>

                    <div class='mild'>
                        <i class="fa fa-star"></i><i class="fa fa-star"></i>
                        <div>Mild</div>
                    </div>

                    <div class='medium'>
                        <i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i>
                        <div>Medium</div>
                    </div>

                    <div class='hot'>
                        <i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i>
                        <div>Spicy</div>
                    </div>

                    <div class='extra-hot'>
                        <i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i>
                        <div>Extra-Spicy</div>
                    </div>
                </div>


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

                        name: 'Seafood Tofu Soup',

                        description: 'Clam & Shrimp',

                        price: 13,

                        isDescription: true

                    },

                    {
                        id: 2,

                        name: 'Combo Tofu Soup',

                        description: 'Clam, Shrimp & Beef',

                        price: 13,

                        isDescription: true

                    },

                    {
                        id: 4,

                        name: 'Kimchi Tofu Soup',

                        price: 13,

                        isVege: true,

                    },

                    {
                        id: 5,

                        name: 'Kimchi Beef Tofu Soup',

                        price: 13

                    },

                    {
                        id: 6,

                        name: 'Kimchi Pork Tofu Soup',

                        price: 13

                    },

                    {
                        id: 8,

                        name: 'Beef Tofu Soup',

                        price: 13

                    },

                    {
                        id: 9,

                        name: 'Pork Tofu Soup',

                        price: 13

                    },

                    {
                        id: 11,

                        name: 'Vegetable Tofu Soup',

                        description: 'Zucchini, Mushroom & Onion, prepared w/ veggie broth',

                        price: 13,

                        isVege: true,

                        isDescription: true,

                    },

                ]

            }

        }

    }

</script>

<style type="text/css">
    .spicy {
        /*width: 375px;*/
        /*margin: 0 auto;*/
    }
    .spicy div{
        /*display: inline-block;*/
       /* display: grid;
        grid-template-columns: repeat(5, 70px);
        text-align:center;
        grid-template-areas:
            "non-spicy mild medium hot extra-hot"*/
    }
    .non-spicy {
        /*grid-area: non-spicy*/
    }
    .mild {
        /*grid-area: mild*/
    }
    .medium {
        /*grid-area: medium*/
    }
    .hot {
        /*grid-area: hot*/
    }
    .extra-hot {
        /*grid-area: extra-hot*/
    }
</style>
