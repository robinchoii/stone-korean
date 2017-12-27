<template>
    <div class='columns'>
        <div class='column'>
            <div class='fish-header'>
                <h2>Grilled Fish</h2>
                <div class='fish-about'>
                    <p>Served with a sizzling hot stone pot rice & side dishes.</p>
                </div>

            </div>
            <div class='fish-flex-grid'>

                <div class='fish-item-card card'>

                    <h3 class='item-title'>Grilled Mackerel</h3>

                    <p class='item-description'>Grilled mackerel with lemon and rice</p>

                    <span class='item-price'>$15</span>

                </div>

                <div class='fish-item-card card'>

                    <h3 class='item-title'>Grilled Flounder</h3>

                    <p class='item-description'>Grilled flounder with lemon and rice</p>

                    <span class='item-price'>$15</span>

                </div>

            </div>

        </div>

    </div>

</template>

<script type="text/javascript">

</script>

<style type="text/css">

    .fish-flex-grid {
        display: grid;

        grid-template-columns: 50% 50%;

        grid-template-rows: 50% 50%;

    }

    .fish-header {
        font-size: 1.5em;

        text-align: center;

        background-color: yellow;

    }

    .fish-item-card {
        text-align: center;

        padding: 15px;

        margin: 5px;
    }

    .fish-about {
        font-size: .6em;

        line-height: 1;
    }
</style>
