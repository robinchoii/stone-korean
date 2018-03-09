<template>

    <div class='google-map' id="stone-map"></div>

</template>

<script type="text/javascript">


    export default {
        name: 'google-map',
        props: ['name'],
        data: function() {
            return {
                mapName: this.name+ "-map",
            }
        },

        mounted: () => {
            const element = document.getElementById('stone-map')
            const options = {
                zoom: 15,
                center: new google.maps.LatLng(47.671285,-122.114915)
            }

            const map = new google.maps.Map(element, options);

            const coordinates = new google.maps.LatLng(47.671285,-122.114915)

            const marker = new google.maps.Marker({
                coordinates

            })

            marker.setMap(map)

        }

    }


</script>

<style type="text/css">
    .google-map {
        width: 800px;
        height: 600px;
        margin: 0 auto;
        background: gray;

    }
</style>
