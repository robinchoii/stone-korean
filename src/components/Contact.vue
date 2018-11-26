<template>
    <div>
        <h1 style='text-align:center;'>How to Reach Us</h1>
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
                    <div class='address'>
                        <div><i class="fa fa-2x fa-location-arrow"></i></div>
                        <a href='https://www.google.com/maps/place/Stone+Korean+Restaurant/@47.6712848,-122.1171033,17z/data=!3m1!4b1!4m5!3m4!1s0x549072b0849aab65:0x323ab2d85984f5b!8m2!3d47.6712848!4d-122.1149146'>16857 Redmond Way<br>
                        Redmond, WA 98052</a>
                    </div>
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
                    <div class='address'>
                        <div><i class="fa fa-2x fa-location-arrow"></i></div>
                        <a href='https://www.google.com/maps/place/Stone+Korean+Restaurant/@47.6272525,-122.3443252,17z/data=!3m1!4b1!4m5!3m4!1s0x549015f23eacc7df:0x6f755914399c427d!8m2!3d47.6272525!4d-122.3421365'>900 Dexter Ave N<br>Seattle, WA 98109</a>
                    </div>
                </div>
                <div class="info-card">
                    <div class='phone'>
                        <div><i class="fa fa-2x fa-phone"></i></div>
                        <a href='tel:+12067172864'>206-717-2864</a>
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

    @media only screen and (max-width: 735px) {
        .info-card {
            margin: 15px 15px;
        }
    }
</style>

