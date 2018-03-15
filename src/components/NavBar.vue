<template>
    <div>

        <a href="/">

            <div class='navbar'>

                <h1>
                    <span>S</span><span>T</span><span>O</span><span>N</span><span>E</span>
                </h1>

                <span class='bar'></span>

                <h4> KOREAN RERSTAURANT </h4>

            </div>
        </a>

    </div>

</template>

<script>

    export default {

    }

</script>

<style type="text/css">
    .navbar {
        display: grid;
        grid-template-columns: 1fr auto 1fr;
        grid-template-rows: auto auto auto;
        background-color: #141212;
        color: white;
        -webkit-text-fill-color: #141212; /* Will override color (regardless overflow: f order) */
        -webkit-text-stroke-width: 2px;
        font-size: 1.5em;
        font-family: 'Rammetto One', cursive;
        line-height: 1.5;
        text-align: center;
        padding: 5px;
        /*border: 3px solid red;*/
    }

    .navbar h1 {
        display: flex;
        justify-content: space-around;
        grid-auto-flow: column;
        grid-column: 2;
        margin: 0;
     }

    .navbar h4 {
        grid-column: 2;
        -webkit-text-stroke-width: 1px;
        margin: 0;
    }

    .bar {
        border: 1px solid white;
        border-radius: 1px;
        height: 3px;
        grid-column: 2;
        background: #ca2626;
     }

     a {
        text-decoration: none;
     }
</style>
