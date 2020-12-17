<template>
    <div class="row mt-md-5 mt-sm-5 mt-xs-5">

        <div class="col-lg-6 col-xs-12" v-for="(newsd, index) of news" :key="index">
            <div class="d-flex justify-content-start">

                <div class="p-3" style="max-width: 300px; aling-self:start">
                    <img :src="newsd.image" alt="" class="col aling-self-start">
                </div>

                <div class="p-2">   
                    <h5>{{newsd.title}}</h5>
                    <p>{{newsd.description}}</p>
                </div>

            </div>
            <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
                <button type="button" class="btn btn-outline-info"><a v-bind:href="newsd.url" target="_blank">Info</a></button>
            </div>
        </div>
    </div>
</template>

<script>
import axios from "axios"

export default {
    name: "NewsSection",
    data(){
        return {news : null}
    },
    created(){
        axios
        .get('https://gnews.io/api/v4/search?q=health&max=4&lang=es&token=5a056159c1ba625a59dd263d281799f7')
        .then(response => {this.news = response.data.articles})
        
    }
}
</script>


<style scoped>

.row mt-md-5 mt-sm-5 mt-xs-5{
    border: 5px blue block;
}

.col-lg-6 col-xs-12{
    border: 5px blue block;
}
</style>
