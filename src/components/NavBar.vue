<template>
    <div>

        <a href="/">

            <div class='navbar'>

                <div class='upper-header'>

                    <span>S</span><span>T</span><span>O</span><span>N</span><span>E</span>

                </div>

                <span class='bar'></span>

                <div class='lower-header'> KOREAN RESTAURANT </div>

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
        -webkit-text-stroke-width: 3px;
        font-family: 'Rammetto One';
        line-height: 1.5;
        text-align: center;
        padding: 5px;
    }

    .navbar .upper-header {
        display: flex;
        justify-content: space-around;
        grid-auto-flow: column;
        grid-column: 2;
        margin: 0;
        font-size: 40px
     }

    .navbar .lower-header {
        grid-column: 2;
        -webkit-text-stroke-width: 1px;
        margin: 0;
        font-size: 30px
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
