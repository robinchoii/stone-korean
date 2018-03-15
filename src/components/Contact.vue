<template>
    <div class='info'>
        <div class='contact-header'>Contact Us</div>

        <div class='hours'>
            <i class="fa fa-clock-o fa-3x"></i>
            <ul>
                <li>Mon - Thur: 11AM - 9:30PM</li>
                <li>Fri - Sun: 11AM - 10PM </li>
                <li>Sun: 11AM - 9PM</li>
            </ul>
        </div>

        <div class='address'>
            <i class="fa fa-location-arrow fa-3x"></i>
            <a href='https://www.google.com/maps/place/Stone+Korean+Restaurant/@47.6712848,-122.1171033,17z/data=!3m1!4b1!4m5!3m4!1s0x549072b0849aab65:0x323ab2d85984f5b!8m2!3d47.6712848!4d-122.1149146'>16857 Redmond Way<br>
            Redmond, WA 98052</a>
        </div>

        <div class='phone'>
            <i class="fa fa-phone fa-3x"></i>
            <a href='tel:+14254970515'>425-497-0515</a>
        </div>
    </div>

</template>

<script>

export default {

  name: 'Contact',

  data () {
    return {

    }
  }
}
</script>

<style lang="css" scoped>

    .info {
        display: grid;
        grid-row-gap: 30px;
        grid-template-areas:
            ". header header header ."
            ". phone hours address .";
        grid-template-columns columns: repeat(auto-fit, minmax(200px, 1fr));
        text-align: center;
        /*align-items: center;*/
        color: white;
        background-color: #141212;
        padding-bottom: 20px;
        margin: auto;
    }
    .info .contact-header {
        grid-area: header;
    }

    .info div {
        font-weight: 600;
        /*line-height: 1*/
    }
    .hours {
        display:grid;
        grid-template-rows: 75px;
        grid-area: hours;
        letter-spacing: 2px;
    }

    .hours ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
    }
    .phone {
        display:grid;
        grid-template-rows: 75px;
        grid-area: phone;
    }

    .phone a, .address a {
        color: white;
        text-decoration: none;
        font-size: 20px;
        letter-spacing: 2px;
    }

    .address {
        grid-area: address;
        display:grid;
        grid-template-rows: 75px;
    }

    .address div, .phone div, .hours ul li {
        font-size: 20px;
    }

    .contact-header {
        font-size: 40px;
    }

    @media only screen and (max-width: 600px) {
        .info {
            grid-template-areas:
                "header"
                "phone"
                "hours"
                "address";
        }

    }

</style>
