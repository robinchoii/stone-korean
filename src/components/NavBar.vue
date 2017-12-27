<template>

    <div>
        <div class="navbar-brand">

            <h1 class="navbar-item title">

                {{name}}

            </h1>

        </div>

        <div class="tabs is-centered">
            <ul>
                <li class="is-active"><a>Home</a></li>
                <li><a>Menu</a></li>
                <li><a>Location</a></li>
                <li><a>Contact</a></li>
            </ul>
        </div>
    </div>

  <!--   <nav class="navbar">

        <div class="navbar-brand">

            <h1 class="navbar-item title" href="/">

                {{name}}

            </h1>

        </div>

        <div class="navbar-menu">

            <div class='navbar-start'>

                <h3 class='navbar-item'>Korean BBQ & Tofu</h3>

            </div>

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

    </nav> -->

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
        background-color: blue
    }

    .nav-item {

        padding: 15px;

    }


</style>
