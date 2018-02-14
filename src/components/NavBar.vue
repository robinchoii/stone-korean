<template>
    <div>


        <div class='navbar'>

            <h1>

                {{name}}

            </h1>

        </div>


        <div class="">

            <a class="" href="/">

                Home

            </a>

            <a class="" href="/">

                Lunch Specials

            </a>

            <a class="" href="/">

                Full Menu

            </a>

            <a class="" href="/">

                Locations


            </a>

        </div>

    </div>

</template>

<script>

    export default {

        data() {
            return {

                name: "Stone Korean Restaurant"

            }
        }


    }

</script>

<style type="text/css">
    .navbar {
        /*background-color: blue*/
    }

    .nav-item {

        padding: 15px;

    }


</style>
