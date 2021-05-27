<template>
    <div>
        <h1 style='text-align:center;'>How to Reach Us</h1>

        <div style='text-align:center;'>
            <p>Please reach out to <br/> <a style='text-decoration:none;color:#e2e2e2;' href='mailto:stonekoreanrestaurant@gmail.com'>stonekoreanrestaurant@gmail.com</a></p>
        </div>

        <div class='info-container'>
            <div class='info-redmond' style='text-align:center;'>
                <h2>Redmond</h2>
                <div class="info-card">
                    <div class='hours'>
                        <div><i class="fa fa-2x fa-clock-o"></i></div>
                        <div><b>Monday - Thursday:</b> <br>11AM - 9:30PM</div>
                        <div><b>Friday - Saturday:</b> <br>11AM - 10PM </div>
                        <div><b>Sunday:</b> <br>11AM - 9PM</div>
                    </div>
                </div>
                <div class="info-card">
                    <a href='https://goo.gl/maps/iHff5CKSHfYoGWYR7'>
                        <div class='address'>
                            <div><i class="fa fa-2x fa-location-arrow"></i></div>
                            <div>16857 Redmond Way</div><br>
                            <div>Redmond, WA 98052</div>
                        </div>
                    </a>
                </div>
                <div class="info-card">
                    <div class='phone'>
                        <div><i class="fa fa-2x fa-phone"></i></div>
                        <a href='tel:+14254970515'>425-497-0515</a>
                    </div>
                </div>
            </div>
            <div class='info-seattle' style='text-align:center;'>
                <h2>Seattle</h2>
                <div class="info-card">
                    <div class='hours'>
                        <div><i class="fa fa-2x fa-clock-o"></i></div>
                        <div><b>Monday - Thursday:</b><br> 11AM - 9:30PM</div>
                        <div><b>Friday - Saturday:</b><br> 11AM - Midnight </div>
                        <div><b>Sunday:</b><br> Closed</div>
                    </div>
                </div>
                <div class="info-card">
                    <a href='https://goo.gl/maps/Ga7t8o45xo68WuCf8'>
                        <div class='address'>
                            <div><i class="fa fa-2x fa-location-arrow"></i></div>
                            <div>900 Dexter Ave N</div><br>
                            <div>Seattle, WA 98109</div>
                        </div>
                    </a>
                </div>
                <div class="info-card">
                    <div class='phone'>
                        <div><i class="fa fa-2x fa-phone"></i></div>
                        <a href='tel:+12067172864'>206-717-2864</a>
                    </div>
                </div>
            </div>
            <div class='info-bothell' style='text-align:center;'>
                <h2><span class='new-location'>New!</span>Bothell</h2>
                <div class="info-card">
                    <div class='hours'>
                        <div><i class="fa fa-2x fa-clock-o"></i></div>
                        <div><b>Monday - Thursday:</b><br> 11AM - 8:00PM</div>
                        <div><b>Friday - Saturday:</b><br> 11AM - 8:30PM </div>
                        <div><b>Sunday:</b><br> 11AM - 8:00PM</div>
                    </div>
                </div>
                <div class="info-card">
                    <a href='https://goo.gl/maps/ud8pPSQbjz9NYiwD7'>
                        <div class='address'>
                            <div><i class="fa fa-2x fa-location-arrow"></i></div>
                            <div>24032 Bothell Everett Hwy Suite #400</div>
                            <div>Bothell, WA 98021</div>
                        </div>
                    </a>
                </div>
                <div class="info-card">
                    <div class='phone'>
                        <div><i class="fa fa-2x fa-phone"></i></div>
                        <a href='tel:+14254081462'>425-408-1462</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script type="text/javascript" charset="utf-8" async defer></script>

<style type="text/css" media="screen">
    .info-container {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(auto, 300px));
        grid-gap: 15px;
        justify-content: center;
    }

    .info-card {
        /* Add shadows to create the "card" effect */
        background-color: #00000073;
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        padding: 25px;
        margin: 15px 0px;
    }

    .info-card a {
        text-decoration: none;
        color: #e2e2e2;
    }
    /* On mouse-over, add a deeper shadow */
    .info-card:hover {
        box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
    }

    .info-card div {
        margin: 3px;
    }

    .new-location {
        margin-right: 5px;
        color: #caae00;
        font-size: 14px;
        position: relative;
        top: 0;
    }

    @media only screen and (max-width: 735px) {
        .info-card {
            margin: 15px 15px;
        }
    }
</style>

