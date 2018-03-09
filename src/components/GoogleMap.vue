<template>


    <div class='google-map' id="stone-map"></div>


</template>

<script type="text/javascript">

    export default {
        name: 'google-map',

        props: ['name'],

        data: () => {
            return {

            }
        },

        mounted: function() {
            const element = document.getElementById('stone-map')
            const options = {
                zoom: 15,
                center: new google.maps.LatLng(47.671285,-122.114915)
            }
            const map = new google.maps.Map(element, options);

            const position = new google.maps.LatLng(47.671285,-122.114915)

            const marker = new google.maps.Marker({
                position: position,
                title:'Stone Korean Restaurant'
            })

            marker.setMap(map)

        }

    }


</script>

<style type="text/css">
    .google-map {
        width: 600px;
        height: 400px;
        margin: 0 auto;
        background: gray;

    }
</style>
