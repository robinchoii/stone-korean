<template>

    <div class='columns'>

        <div class='column'>

            <div class='combo-specials-header'>

                <h2>Combo Specials</h2>

                <div class='combo-specials-about'>

                    <p>Served with a sizzling hot stone pot rice except 1,2,3,9,& 10 and assortment of side dishes.</p>

                    <p>(1 person serving, samller portions than if ordered separately)</p>

                </div>

            </div>

            <div class='combo-specials-flex-grid'>

                <div class='combo-special-item-card card '>
                    <span class='num is-pulled-left'>1</span>
                    <h3 class='item-title'>Bulgogi or Spicy Pork + Hotpot Bibimbob</h3>

                    <p class='item-description'></p>

                    <span class='item-price'>$23</span>

                </div>

                <div class='combo-special-item-card card'>
                    <span class='num is-pulled-left'>2</span>

                    <h3 class='item-title'>Kalbi(Short Ribs) + Hotpot Bibimbob</h3>

                    <p class='item-description'></p>

                    <span class='item-price'>$25</span>

                </div>

                <div class='combo-special-item-card card'>
                    <span class='num is-pulled-left'>3</span>

                    <h3 class='item-title'>Soft Tofu Soup + Hotpot Bibimbob</h3>

                    <p class='item-description'></p>

                    <span class='item-price'>$23</span>

                </div>

                <div class='combo-special-item-card card'>
                    <span class='num is-pulled-left'>4</span>

                    <h3 class='item-title'>Bulgogi + Soft Tofu Soup + Stone Rice</h3>

                    <p class='item-description'></p>

                    <span class='item-price'>$23</span>

                </div>

                <div class='combo-special-item-card card'>
                    <span class='num is-pulled-left'>5</span>

                    <h3 class='item-title'>Spicy Pork + Soft Tofu Soup + Stone Rice</h3>

                    <p class='item-description'></p>

                    <span class='item-price'>$23</span>

                </div>

                <div class='combo-special-item-card card'>
                    <span class='num is-pulled-left'>6</span>

                    <h3 class='item-title'>Chicken Bulgogi + Soft Tofu Soup + Stone Rice</h3>

                    <p class='item-description'></p>

                    <span class='item-price'>$23</span>

                </div>

                <div class='combo-special-item-card card'>
                    <span class='num is-pulled-left'>7</span>

                    <h3 class='item-title'>Spicy Chicken Bulgogo + Soft Tofu Soup + Stone Rice</h3>

                    <p class='item-description'></p>

                    <span class='item-price'>$23</span>

                </div>

                <div class='combo-special-item-card card'>
                    <span class='num is-pulled-left'>8</span>

                    <h3 class='item-title'>Kalbi (Short Ribs) + Soft Tofu Soup + Stone Rice</h3>

                    <p class='item-description'></p>

                    <span class='item-price'>$24</span>

                </div>

                <div class='combo-special-item-card card'>
                    <span class='num is-pulled-left'>9</span>

                    <h3 class='item-title'>Kalbi (Short Ribs) + Naeng-Myun(Cold Noodle Soup)</h3>

                    <p class='item-description'></p>

                    <span class='item-price'>$24</span>

                </div>

                <div class='combo-special-item-card card'>
                    <span class='num is-pulled-left'>10</span>

                    <h3 class='item-title'>Chicken Bulgogi + Hotpot Bibimbob</h3>

                    <p class='item-description'></p>

                    <span class='item-price'>$3</span>

                </div>

            </div>

        </div>

    </div>

</template>

<script type="text/javascript">

    export default {

    }
</script>

<style type="text/css">

    .combo-specials-header {
        font-size: 1.5em;

        text-align: center;

        background-color: yellow;

    }

    .combo-specials-about {
        font-size: .6em;

        line-height: 1;

    }

    .combo-specials-flex-grid {
        display: grid;

        grid-template-columns: 50% 50%;

        grid-template-rows: 50% 50%;

        margin: auto;

    }

    .combo-special-item-card {
        text-align: center;

        padding: 15px;

        margin: 5px;

        position: relative;

    }

    .num {
        font-size: 1em
    }

</style>
