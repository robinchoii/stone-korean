<template>
    <div class='catering-container'>
        <div>
            If you have any questions about Catering
        </div>

        <div>
            Email <a class='email' href='mailto:stonekoreanrestaurant@gmail.com'>stonekoreanrestaurant@gmail.com</a> or call <a class='phone' href="tel:+14254970515" title="">425-497-0515</a>
        </div>

    </div>
</template>

<script>
    export default {

      name: 'Catering',

      data () {
        return {

        }
      }
    }
</script>

<style lang="css" scoped>
    .catering-container {
        display: grid;
        grid-template-columns: auto-fit;
        justify-items: center;
        /*border: 3px solid black;*/
        padding: 50px;
        text-align: center;
        color: #e2e2e2;
        font-weight: 700;
    }

    .email, .phone{
        color: #e9e993;
    }

</style>
