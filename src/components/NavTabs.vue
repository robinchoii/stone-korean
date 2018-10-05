<template>

    <div class='nav-tabs'>

        <div class='tabs'>

            <ul>

                <li><a href="/" title="">Home</a></li>

                <li><a href="#contact" title="">Contact</a></li>
                <li @click="toggleRedmondTab">
                    Redmond
                    <ul v-if="isRedmond">
                        <li @click='toggleRedmondMenu'>
                            Menu
                        </li>
                        <li @click='toggleOrderOnlineTab'>
                            Order Online
                            <dropdown v-if='isOrderOnline'></dropdown>

                        </li>
                    </ul>
                </li>
                <li @click='toggleSeattleTab'>
                    Seattle
                    <ul v-if='isSeattle'>
                        <li class='menu-list' @click='toggleSeattleMenu'>
                            <span id='menu'>Menu</span>
                            <ul class="" v-for='tab in tabs' v-show='isSeattleMenuOpen'>

                                <li>

                                    <a  :class="{'is-active' : tab.isActive}" :href='tab.href' @click='selectTab(tab)'>{{tab.name}} {{tab.title}}</a>

                                </li>

                            </ul>

                        </li>
                    </ul>
                </li>

            </ul>

        </div>


        <div class='tabs-details'>

            <full-menu v-if='isRedmondMenuOpen'> </full-menu>

        </div>

    </div>

</template>

<script>

import Dropdown from './Dropdown.vue'
import FullMenu from './FullMenu.vue'

export default {

    components: {

        Dropdown, FullMenu

    },

  name: 'NavTabs',

  data () {
    return {
        tabs: [],
        isRedmondMenuOpen: false,
        isSeattleMenuOpen: false,
        isOrderOnline: false,
        isRedmond: false,
        isSeattle: false
    }
  },

  created() {
    this.tabs = this.$children
  },


  methods: {
    selectTab(selectedTab) {
        this.tabs.forEach( tab => {
            tab.isActive = (tab.name == selectedTab.name);
        })
        console.log(window.location.href)
    },
    toggleRedmondMenu(tab) {
        // if (this.isMenuOpen === false) {
        //     this.isMenuOpen = true
        // }
        console.log('click')
        tab.stopPropagation()
        this.isRedmondMenuOpen = !this.isRedmondMenuOpen

        return false
    },
    toggleSeattleMenu(tab) {
        // if (this.isMenuOpen === false) {
        //     this.isMenuOpen = true
        // }
        console.log('click')
        tab.stopPropagation()
        this.isSeattleMenuOpen = !this.isSeattleMenuOpen

        return false
    },
    toggleOrderOnlineTab() {
        event.stopPropagation();
        this.isOrderOnline = !this.isOrderOnline

        return false;
    },
    toggleRedmondTab(event) {
        event.stopPropagation()
        this.isRedmond = !this.isRedmond

        return false;
    },
    toggleSeattleTab(event) {
        event.stopPropagation()
        this.isSeattle = !this.isSeattle

        return false;
    },
    openMenu(event) {
        event.stopPropagation();

        this.isMenuOpen = !this.isMenuOpen

    }
  }

}
</script>

<style lang="css" scoped>
    .nav-tabs {
/*        display: grid;
        grid-template-columns: minmax(300px, 1fr);
        grid-gap: 25px;
        grid-template-areas:
            "tabs"
            "tabs-detail"*/
            display: grid;
            grid-template-areas:
                "left-nav main-menu";
    }
    .tabs  {
        grid-area: left-nav;
        letter-spacing: 0px;
        padding: 15px 0 15px 0;
        background-color: #3d1b1b !important;
        width: 110px;

     }
        .tabs ul {
            margin: 0;
            padding: 0;
        }

     .tabs-details{
        grid-area: main-menu;
        letter-spacing: 2px;

     }

    .tabs ul li {
        font-size: 16px;
        list-style-type: none;
        line-height: 2.5;
        text-transform: uppercase;
        color: #e2e2e2;
        margin: 0px;
        padding: 0px;
        line-height: 1.65;

    }
    .tabs ul li a {
        text-decoration: none;
        color: #e2e2e2;
        font-weight: 700;
    }


    .is-active {
        border-bottom: 4px solid #c71b00;
    }

    .tabs, .tabs-detail {
        background-color: #3d1b1b;
        color: #e2e2e2;
    }

    .tab-details {
        max-width: 1200px;
    }

    #menu {
        font-weight: 700;
        grid-column: 1;
    }

/*    .menu-list ul {
        grid-row: 2;
    }*/

    .menu-list ul li a  {
        /*color: ;*/
    }

    .order-online {
        display: block;
    }

    .tabs ul li {
        margin-left: 4px;
        margin-right: 15px;
    }
</style>
