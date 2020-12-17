<template>
   <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
        <ol class="carousel-indicators">
            <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
        </ol>
        <div class="carousel-inner">
            <div class="carousel-item active" style="height: 50vh">
                    <img class="d-block img-fluid" src="https://i.imgur.com/SrQSn5t.png" alt="First slide" style="width: 100%;">

                <div class="carousel-caption d-none d-md-block">
                    <h1>Un mate</h1>
                    <h3>siempre es una buena idea</h3>
                </div>
            </div>
            <div class="carousel-item" style="height: 50vh"> 
                
                    <img class="d-block img-fluid" src="https://i.imgur.com/4hhSXV5.png" alt="Second slide">

                <div class="carousel-caption d-none d-md-block">
                    <h1>¡De origen natural!</h1>
                    <h3>Energía, tranquilidad, buenas conversaciones, todo eso y más cabe en un mate</h3>
                </div>
            </div>
            <div class="carousel-item" style="height: 50vh">
                
                <title>Placeholder</title>
                    <img class="d-block img-fluid" src="https://i.imgur.com/Ley7BrB.png" alt="Third slide">

                <div class="carousel-caption d-none d-md-block">
                    <h1>Disfruta lo simple</h1>
                </div>
            </div>
        </div>
        <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
        </a>
    </div>
</template>

<script>

export default {
    name: "Carousel",
}
</script>

<style scoped>

</style>