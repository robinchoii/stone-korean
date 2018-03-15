<template>

    <div class='nav-tabs'>

        <div class='tabs'>

            <ul>

                <li v-for='tab in tabs' :class="{'is-active' : tab.isActive}">

                    <a :href='tab.href' @click='selectTab(tab)'>{{tab.name}} {{tab.title}}</a>

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
        tabs: []
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
    }
  }


}
</script>

<style lang="css" scoped>
    .nav-tabs {
        display: grid;
        grid-template-columns: auto 1fr;
        grid-gap: 50px;
        grid-template-areas:
            "tabs tabs-detail"
    }
    .tabs  {
        grid-area: tabs;
     }

     .tabs-detail{
        grid-area: tabs-details;
     }

    .tabs ul li {
        font-size: 16px;
        list-style-type: none;
        line-height: 3;

    }
    .tabs ul li a {
        text-decoration: none;
        color: #e2e2e2;
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

    @media only screen and (max-width: 600px) {
        .nav-tabs {
            grid-template-columns: 1fr;
            grid-template-areas:
                "tabs"
                "tabs-detail"
        }

        .tabs ul {
            display: grid;
            /*grid-row-gap: 50px;*/
            grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
        }
    }
</style>
