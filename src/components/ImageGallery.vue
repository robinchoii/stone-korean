<template>
    <div class='gallery'>


    </div>
</template>

<script>
    const ImageGallery = document.querySelector('.gallery');

    generateHTML () => {
        return `
            <div>
                <img src='../assets/stone${generateNumber}.jpg' alt='food'>
            </div>
        `
    }

    generateNumber () => {
        for (var i = 1; i < 25; i++) {
            return i
        }
    }


    export default {

      name: 'ImageGallery',

      data () {
        return {

        }
      }
    }
</script>

<style lang="css" scoped>
</style>
