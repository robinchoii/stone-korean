<template>

    <div class='nav-tabs'>

        <div class='tabs'>

            <ul>

                <li><a href="/" title="">Home</a></li>

                <li><a href="#contact" title="">Contact</a></li>

                <li class='menu-list' @click='toggleMenu'>
                    <span id='menu'>Menu</span>
                    <ul class="" v-for='tab in tabs' v-show='isMenuOpen'>

                        <li  :class="{'is-active' : tab.isActive}">

                            <a :href='tab.href' @click='selectTab(tab)'>{{tab.name}} {{tab.title}}</a>

                        </li>

                    </ul>

                </li>

            </ul>

        </div>


        <div class='tabs-details'>

            <slot></slot>

        </div>

    </div>

</template>

<script>
export default {

  name: 'NavTabs',

  data () {
    return {
        tabs: [],
        isMenuOpen: false
    }
  },

  created() {
    this.tabs = this.$children
  },


  methods: {
    selectTab(selectedTab) {
        // alert('selecting')
        this.tabs.forEach( tab => {
            tab.isActive = (tab.name == selectedTab.name);
        })
        console.log(window.location.href)
    },
    toggleMenu(tab) {
        console.log(tab)
        if (this.isMenuOpen === false) {
            this.isMenuOpen = true
        }
    }
  }


}
</script>

<style lang="css" scoped>
    .nav-tabs {
        display: grid;
        grid-template-columns: minmax(300px, 1fr);
        grid-gap: 25px;
        grid-template-areas:
            "tabs"
            "tabs-detail"
    }
    .tabs  {
        grid-area: tabs;
        letter-spacing: 0px;

     }
        .tabs ul {
            margin: 0;
            padding: 0;
        }

     .tabs-detail{
        grid-area: tabs-details;
        letter-spacing: 2px;
     }

    .tabs ul li {
        font-size: 16px;
        list-style-type: none;
        line-height: 2.5;
        text-transform: uppercase;
        color: #c8a5aa;
        margin: 0px;
        padding: 0px;
        text-align: center;
        line-height: 1.65;

    }
    .tabs ul li a {
        text-decoration: none;
        color: #c8a5aa;
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

    .menu-list ul {
        grid-row: 2;
    }

    .menu-list ul li a  {
        /*color: ;*/
    }



    @media only screen and (min-width: 800px) {
        .menu-list {
            display:flex;
            /*grid-template-columns: repeat(auto-fill, minmax(auto,1fr));*/
            /*grid-column-gap: 5px;*/
        }

        .tabs ul {
            display: grid;
            grid-auto-flow: column;
            grid-gap: 20px;
            grid-template-columns: repeat(auto-fit, minmax(auto, 1fr));
            justify-content: left;

        }

        .tabs ul li {
            margin-left: 4px;
            margin-right: 15px;
        }
    }
</style>
