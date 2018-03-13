<template>

    <div>

        <div class='tabs'>

            <ul>

                <li v-for='tab in tabs' :class="{'is-active' : tab.isActive}">

                    <a :href='tab.href' @click='selectTab(tab)'>{{tab.name}}</a>

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

    .tabs ul li {
        list-style-type: none;
    }
    .tabs ul li a {
        text-decoration: none;
        color: red;
    }

    .tabs ul {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(100px, 1fr))
    }

    .is-active {
        background: purple;
    }
</style>
