<template>
    <div>
        <h1 style='text-align:center;'>Where to?</h1>
        <div class='online-order-container'>
            <h2>Redmond</h2>
            <h2>Seattle</h2>
            <div class="order-card">
                <a href="https://www.trycaviar.com/t/seattle-eastside/stone-korean-8604?groups=f_online__d_dwidget-4-button-1__p_marketing__c_merchant-links&how=pickup&utm_medium=localmarketing&utm_source=widget&utm_campaign=stone-korean-8604&utm_term=seattle-eastside&utm_content=stone-korean-8604&cvosrc=localmarketing.widget.stone-korean-8604&cvo_campaign=stone-korean-8604&cav_source=stone-korean-8604&cav_medium=widget">
                    <div class="order-wrapper">
                        <h3>Pick&nbsp;Up</h3>
                        <i class="fa fa-4x fa-shopping-bag" aria-hidden="true"></i>
                    </div>
                </a>
            </div>

            <div class="order-card">
              <div class="order-wrapper">
                <h3>Coming Soon!</h3>
                <i class="fa fa-4x fa-shopping-bag" aria-hidden="true"></i>
              </div>
            </div>

            <div class="order-card">
                <a href="https://www.trycaviar.com/t/seattle-eastside/stone-korean-8604?groups=f_online__d_dwidget-4-button-1__p_marketing__c_merchant-links&how=delivery&utm_medium=localmarketing&utm_source=widget&utm_campaign=stone-korean-8604&utm_term=seattle-eastside&utm_content=stone-korean-8604&cvosrc=localmarketing.widget.stone-korean-8604&cvo_campaign=stone-korean-8604&cav_source=stone-korean-8604&cav_medium=widget">
                    <div class="order-wrapper">
                        <h3>Caviar</h3>
                        <i class="fa fa-4x fa-car" aria-hidden="true"></i>
                    </div>
                </a>
            </div>

            <div class="order-card">
                <a href="https://www.ubereats.com/en-US/seattle/food-delivery/stone-korean-restaurant-dexter-ave/eLYGmDkSQ9iBcHWvuGjI4g/" title="">
                  <div class="order-wrapper">
                    <h3>Uber Eats</h3>
                    <i class="fa fa-4x fa-car" aria-hidden="true"></i>
                  </div>
                </a>
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

    .order-card a {
        text-decoration: none;
        color: #e2e2e2;
    }
    /* On mouse-over, add a deeper shadow */
    .order-card:hover {
        box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
    }

</style>
