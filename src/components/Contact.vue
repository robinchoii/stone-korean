<template>
    <div class='info'>
        <h2>Contact Us</h2>
        <div class='hours'>
            <i class="fa fa-clock-o fa-3x"></i>
            <h4>Mon - Thur: 11AM - 9:30PM</h4>
            <h4>Fri - Sun: 11AM - 10PM </h4>
            <h4>Sun: 11AM - 9PM</h4>

        </div>

        <div class='address'>
            <i class="fa fa-location-arrow fa-3x"></i>
            <h4>16857 Redmond Way<br>
            Redmond, WA 98052</h4>
        </div>

        <div class='phone'>
            <i class="fa fa-phone fa-3x"></i>
            <i class="fas fa-clock"></i>
            <h4>425-497-0515</h4>
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
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        text-align: center;
        align-items: center;
        color: white;
        background-color: black;
    }

    .hours {
        /*grid-column: 2 / 3;*/
    }

    .phone {
        /*grid-column: 4 / 5;*/
    }

    .address {
        /*grid-column: 3 / 4;*/
    }

    .fa-clock-o {
        /*color: red;*/
     }
     .fa-phone {
        /*color: blue;*/
     }
</style>
