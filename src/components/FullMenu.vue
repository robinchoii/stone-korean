<template>
    <div>
        <lunch-menu ></lunch-menu>

        <appetizers-menu> </appetizers-menu>

        <soft-tofu-soup-menu></soft-tofu-soup-menu>

        <bibimbob-menu></bibimbob-menu>

        <bbq-menu></bbq-menu>

        <fried-chicken-menu></fried-chicken-menu>

        <grilled-fish-menu></grilled-fish-menu>

        <sauteed-dishes-menu></sauteed-dishes-menu>

        <combo-specials></combo-specials>

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
        line-height: 1;
        font-size: .75em;
    }

    .item-price {
        color: black;
        font-size:.8em;
        font-weight: 600;
    }

    .item-title {
        font-weight: 600;
        line-height: 1;
        margin-bottom: 3px
    }
</style>
