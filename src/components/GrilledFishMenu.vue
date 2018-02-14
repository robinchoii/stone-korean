<template>
    <div class='fishes'>

        <div class='fishes-header'>

            <h2>Grilled Fish</h2>

            <div class='fish-about'>

                <p>Served with a sizzling hot stone pot rice & side dishes.</p>

            </div>

        </div>

        <div class='fishes-items'>

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

</template>

<script type="text/javascript">

</script>

<style type="text/css">

    .fishes{
        display: grid;
        grid-template-columns: 1fr;
        grid-gap: 20px;

    }

    .fishes-items {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        grid-gap: 1px;
    }

    .fishes-header {
        font-size: 1.5em;

        text-align: center;

        background-color: yellow;

    }

    .fish-item-card {
        padding: 10px;

    }

    .fish-about {
        font-size: .55em;
        line-height: 1;
    }
</style>
