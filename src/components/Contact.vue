<template>
    <div class='info'>
        <div class='contact-header'>Contact Us</div>

        <div class='hours'>
            <i class="fa fa-clock-o"></i>
            <div>Mon - Thur: 11AM - 9:30PM</div>
            <div>Fri - Sun: 11AM - 10PM </div>
            <div>Sun: 11AM - 9PM</div>
        </div>

        <div class='address'>
            <i class="fa fa-location-arrow"></i>
            <a href='https://www.google.com/maps/place/Stone+Korean+Restaurant/@47.6712848,-122.1171033,17z/data=!3m1!4b1!4m5!3m4!1s0x549072b0849aab65:0x323ab2d85984f5b!8m2!3d47.6712848!4d-122.1149146'>16857 Redmond Way<br>
            Redmond, WA 98052</a>
        </div>

        <div class='phone'>
            <i class="fa fa-phone"></i>
            <a href='tel:+14254970515'>425-497-0515</a>
        </div>

        <div class='email'>
            <i class='fa fa-envelope'></i>
            <a href='mailto:stonekoreanrestaurant@gmail.com'>stonekoreanrestaurant@gmail.com</a>
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
        grid-gap: 30px;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        text-align: center;
        color: white;
        background-color: #141212;
        padding-bottom: 20px;
    }

        .info > * i {
            font-size: 40px;
        }

    .contact-header {
        font-size: 36px;
        letter-spacing: 2px;
        grid-column: 1  / -1;
        margin: 20px;
    }

    .phone a, .address a, .email a{
        color: white;
        text-decoration: none;
        letter-spacing: 2px;
    }

    .address, .hours, .phone , .email {
        display: grid;
        grid-template-rows: 50px;
        letter-spacing: 2px;
        font-size: 16px;
    }
</style>
