<template>
    <div class='info'>
        <div id='contact'>Contact Us</div id='contact'>

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
            <div>16857 Redmond Way<br>
            Redmond, WA 98052</div>
        </div>

        <div class='phone'>
            <i class="fa fa-phone fa-3x"></i>
            <div>425-497-0515</div>
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
            "header header header"
            "phone hours address";
        grid-template-columns columns: repeat(auto-fit, minmax(200px, 1fr));
        text-align: center;
        /*align-items: center;*/
        color: white;
        background-color: #141212;
        padding-bottom: 20px;
    }
    .info #contact {
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

    .address {
        grid-area: address;
        display:grid;
        grid-template-rows: 75px;
    }

    .address div, .phone div, .hours ul li {
        font-size: 20px;
    }

    #contact {
        font-size: 40px;
    }

    @media only screen and (max-width: 500px) {
        .info {
            grid-template-areas:
                "header"
                "phone"
                "hours"
                "address";
        }

    }

</style>
