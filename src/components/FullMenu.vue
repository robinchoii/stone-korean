<template>
    <div class='full-menu'>
        <lunch-menu ></lunch-menu>

        <appetizers-menu> </appetizers-menu>

        <soft-tofu-soup-menu></soft-tofu-soup-menu>

        <bibimbob-menu></bibimbob-menu>

        <bbq-menu></bbq-menu>

        <combo-specials></combo-specials>

        <fried-chicken-menu></fried-chicken-menu>

        <sauteed-dishes-menu></sauteed-dishes-menu>

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

    export default {

        components: {

                LunchMenu, AppetizersMenu, SoftTofuSoupMenu, BibimbobMenu, BbqMenu, FriedChickenMenu, GrilledFishMenu, SauteedDishesMenu, ComboSpecials

        },
    }
</script>

<style type="text/css">

    .item-description {
        font-size: .85em;
    }

    .item-price {
        color: black;
        font-size:.9em;
        font-weight: 600;
    }

    .item-title {
        font-weight: 600;
        line-height: 1;
        margin-bottom: 3px;
        text-transform: uppercase;
    }

    .item-card {
        border: solid 2px gray;
        box-shadow: 2px 2px 1px 1px rgba(0, 0, 0, 0.1);
        padding: 10px;
    }

    .item-card > * {
        margin: 0;
        line-height: 1.25;
    }

    .food-wrapper {
        display: grid;
        grid-template-columns: 1fr;
        grid-gap:20px;
    }

    .food-items-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        grid-gap: 10px;
    }
    .main-header {
        padding: 15px;
        background-color: yellow;
    }

    .main-header h2 {
        text-transform: uppercase;
        margin: 10px;

    }

    .main-header h2, .main-header p {
        /*margin: 0;*/
        /*padding: 0;*/
        text-align: center;

    }

    .main-about > *, .vege {
        font-size: .9em;
    }

    .main-header p {
        margin: 0;
        padding: 0;
    }

/*    .full-menu {
        margin: auto 50px;
    }*/
</style>
