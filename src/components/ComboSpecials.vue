<template>

    <div class='combo-specials'>

        <div class='combo-specials-header'>

            <h2>Combo Specials</h2>

            <div class='combo-specials-about'>

                <p>Served with a sizzling hot stone pot rice except 1,2,3,9,& 10 and assortment of side dishes.</p>

                <p>(1 person serving, samller portions than if ordered separately)</p>

            </div>

        </div>

        <div class='combo-specials-items'>

            <div class='combo-special-item-card card '>
                <span class='combo-number'>1</span>
                <h3 class='item-title'>Bulgogi or Spicy Pork + Hotpot Bibimbob</h3>

                <span class='item-price'>$23</span>

            </div>

            <div class='combo-special-item-card card'>
                <span class='combo-number'>2</span>

                <h3 class='item-title'>Kalbi(Short Ribs) + Hotpot Bibimbob</h3>

                <span class='item-price'>$25</span>

            </div>

            <div class='combo-special-item-card card'>
                <span class='combo-number'>3</span>

                <h3 class='item-title'>Soft Tofu Soup + Hotpot Bibimbob</h3>

                <span class='item-price'>$23</span>

            </div>

            <div class='combo-special-item-card card'>
                <span class='combo-number'>4</span>

                <h3 class='item-title'>Bulgogi + Soft Tofu Soup + Stone Rice</h3>

                <span class='item-price'>$23</span>

            </div>

            <div class='combo-special-item-card card'>
                <span class='combo-number'>5</span>

                <h3 class='item-title'>Spicy Pork + Soft Tofu Soup + Stone Rice</h3>

                <span class='item-price'>$23</span>

            </div>

            <div class='combo-special-item-card card'>
                <span class='combo-number'>6</span>

                <h3 class='item-title'>Chicken Bulgogi + Soft Tofu Soup + Stone Rice</h3>

                <span class='item-price'>$23</span>

            </div>

            <div class='combo-special-item-card card'>
                <span class='combo-number'>7</span>

                <h3 class='item-title'>Spicy Chicken Bulgogo + Soft Tofu Soup + Stone Rice</h3>

                <span class='item-price'>$23</span>

            </div>

            <div class='combo-special-item-card card'>
                <span class='combo-number'>8</span>

                <h3 class='item-title'>Kalbi (Short Ribs) + Soft Tofu Soup + Stone Rice</h3>

                <span class='item-price'>$24</span>

            </div>

            <div class='combo-special-item-card card'>
                <span class='combo-number'>9</span>

                <h3 class='item-title'>Kalbi (Short Ribs) + Naeng-Myun(Cold Noodle Soup)</h3>

                <span class='item-price'>$24</span>

            </div>

            <div class='combo-special-item-card card'>
                <span class='combo-number'>10</span>

                <h3 class='item-title'>Chicken Bulgogi + Hotpot Bibimbob</h3>

                <span class='item-price'>$3</span>

            </div>

        </div>

    </div>

</template>

<script type="text/javascript">

    export default {

    }
</script>

<style type="text/css">
    .combo-specials {
        display: grid;
        grid-template-columns: 1fr;
        grid-gap: 20px;
    }

    .combo-specials-header {
        font-size: 1.5em;
        text-align: center;
        background-color: yellow;

    }

    .combo-specials-about {
        font-size: .55em;
        line-height: 1;

    }

    .combo-specials-items {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        grid-gap: 10px;
    }

    .combo-special-item-card {
        display: grid;
        grid-template-columns: auto 1fr;
        padding: 10px;
        grid-column-gap: 15px;
    }

    .combo-special-item-card .item-price {
        grid-column: 2;
    }
</style>
