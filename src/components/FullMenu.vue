f<template>
    <div class='full-menu'>
        <lunch-menu ></lunch-menu>

        <appetizers-menu> </appetizers-menu>

        <soft-tofu-soup-menu></soft-tofu-soup-menu>

        <bibimbob-menu></bibimbob-menu>

        <bbq-menu></bbq-menu>

        <combo-specials></combo-specials>

        <fried-chicken-menu></fried-chicken-menu>

        <sauteed-dishes-menu></sauteed-dishes-menu>

        <fried-rice-menu></fried-rice-menu>

        <cold-noodle-menu></cold-noodle-menu>

        <soups-and-stews-menu></soups-and-stews-menu>

        <grilled-fish-menu></grilled-fish-menu>

    </div>
</template>

<script type="text/javascript">
    import LunchMenu from './LunchMenu.vue'
    import AppetizersMenu from './AppetizersMenu.vue'
    import SoftTofuSoupMenu from './SoftTofuSoupMenu.vue'
    import BibimbobMenu from './BiBimBobMenu.vue'
    import BbqMenu from './BBQMenu.vue'
    import FriedChickenMenu from './FriedChickenMenu.vue'
    import GrilledFishMenu from './GrilledFishMenu.vue'
    import SauteedDishesMenu from './SauteedDishesMenu.vue'
    import ComboSpecials from './ComboSpecials.vue'
    import FriedRiceMenu from './Seattle/FriedRiceMenu.vue'
    import ColdNoodleMenu from './ColdNoodleMenu.vue'
    import SoupsAndStewsMenu from './SoupsAndStewsMenu.vue'

    export default {

        components: {

                LunchMenu, AppetizersMenu, SoftTofuSoupMenu, BibimbobMenu, BbqMenu, FriedChickenMenu, GrilledFishMenu, SauteedDishesMenu, ComboSpecials, FriedRiceMenu, ColdNoodleMenu, SoupsAndStewsMenu

        },
    }
</script>

<style type="text/css">
    .full-menu {
        display: grid;
        grid-template-columns: minmax(300px, 1fr);
        grid-gap: 20px;
        background-color: #3d1b1b;
        letter-spacing: 2px;
        margin-bottom: 50px;
        width: auto;
        margin: 0 auto;
    }

    .item-description {
        font-size: .85em;
        color: #aaa;
        line-height: 1.25
    }

    .item-price {
        color: #e2e2e2;
        text-align: right;
    }

    .item-title {
        font-weight: 600;
        text-transform: uppercase;
    }

    .item-card {
        display: grid;
        grid-template-columns: 1fr 30px;
        grid-template-rows: auto 1fr;
        padding: 10px;
    }

    .item-card > * {
        margin: 0;
    }

    .food-items-grid {
        display: grid;
        justify-content: left;
        grid-template-columns: repeat(auto-fit, minmax(300px, 400px));
        grid-gap: 10px;
    }

    @media only screen and (min-width: 600px) {
        .food-items-grid {
            grid-template-columns: repeat(2, minmax(300px, 400px));
        }
    }

    @media only screen and (max-width: 600px) {
        .main-about > * {
            font-size: 12px !important;
            font-weight: 200;
        }
        .item-title {
            font-size: 15px;
        }
    }
    .main-header {
        padding: 10px;
        text-align: center;
    }

    .main-header h2 {
        text-transform: uppercase;
        margin: 5px;
        color: #caae00;
    }

    .main-header h2, .main-header p {
        margin: 0;
        padding: 0;
        // text-align: center;
    }

    .main-about > p {
        font-size: .9em;
        font-weight: 400;
        color: #aaa;;
    }

    .fa-leaf {
        color: #00ce00;
    }

    .korean-word {
        font-size: 10px;
    }

    @media screen and (min-width: 768px) {
        .full-menu {
            width: 800px;
            margin: 0 auto;
        }
    }

    @media screen and (max-width: 768px) {
        .large {
            display:none;
        }
    }

</style>
