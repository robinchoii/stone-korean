<template>
    <div>
        <h1 style='text-align:center;'>Where to?</h1>
        <div class='online-order-container'>
            <h2>Redmond</h2>
            <h2>Seattle</h2>
            <div class="order-card">
              <div class="order-wrapper">
                <h3>Pick&nbsp;Up</h3>
                <i class="fa fa-4x fa-shopping-bag" aria-hidden="true"></i>
              </div>
            </div>

            <div class="order-card">
              <div class="order-wrapper">
                <h3>Coming Soon!</h3>
                <i class="fa fa-4x fa-shopping-bag" aria-hidden="true"></i>
              </div>
            </div>

            <div class="order-card">
              <div class="order-wrapper">
                <h3>Delivery</h3>
                <i class="fa fa-4x fa-car" aria-hidden="true"></i>
              </div>
            </div>

            <div class="order-card">
              <div class="order-wrapper">
                <h3>Coming Soon!</h3>
                <i class="fa fa-4x fa-car" aria-hidden="true"></i>
              </div>
            </div>
        </div>
    </div>
</template>

<scripttype="text/javascript" charset="utf-8" async defer></script>

<style type="text/css" media="screen">
    .online-order-container {
        margin: 50px auto;
        display: grid;
        grid-template-columns: repeat(2, minmax(auto, 300px));
        grid-gap: 15px;
        text-align: center;
        justify-content: center;
        margin-top: 0;
    }

    .order-card {
    /* Add shadows to create the "card" effect */
        background-color: #00000073;
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    transition: 0.3s;
    padding: 25px;
}

/* On mouse-over, add a deeper shadow */
.order-card:hover {
    box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

</style>
