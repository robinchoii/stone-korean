<template>
    <nav class="navbar">

        <div class="navbar-brand">

            <h1 class="navbar-item title" href="/">

                {{name}}

            </h1>

        </div>

        <div class="navbar-menu">

            <div class="navbar-end">

                <a class="navbar-item" href="/">

                    Home

                </a>

                <a class="navbar-item" href="/">

                    Lunch Specials

                </a>

                <a class="navbar-item" href="/">

                    Full Menu

                </a>

                <a class="navbar-item" href="/">

                    Locations


                </a>

            </div>

        </div>

    </nav>

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

    .nav-item {

        padding: 15px;

    }


</style>
