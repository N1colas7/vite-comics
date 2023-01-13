<script>
    import CardSeries from './CardSeries.vue';
    import dataitems from '../assets/data/dataitems.js';


    export default {
        components:{
            CardSeries
        },
        data() {
            return {
                products: dataitems,
                linkContent:[
                    {
                        label:'Digital Comics',
                        url: "buy-comics-digital-comics.png"
                    },
                    {
                        label:'DC Merchandise',
                        url: "buy-comics-merchandise.png"
                    },
                    {
                        label:'Susbscriptions',
                        url: "buy-comics-subscriptions.png"
                    },
                    {
                        label:'Comic Shop Locator',
                        url: "buy-comics-shop-locator.png"
                    },
                    {
                        label:'DC Power Visa',
                        url: "buy-dc-power-visa.svg"
                    },
                ]
            }
        },
    }
</script>

<template>
    <div>
        <div class="contents-image">
            <div class="jumbo">
                <img src="/img/jumbotron.jpg">
            </div>
            <div class="library-image">
                <div class="row">
                    <CardSeries v-for="(item, index) in products " :key="index" :serie="item"/>
                    <CardSeries />
                </div>        
             </div>   
        </div>
    </div>
    <div class="linkContent-container">
        <ul>
            <li v-for="(link, i) in linkContent" :key="i">
                    <img class="image" :src="`/img/${link.url}`" alt="image" >
                    <a class="text-image" :href= link.label>{{ link.label }}</a>
            </li>
        </ul>   
    </div>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    .contents-image{
        background-color: black;
        color:white;
        width: 100%;
    }
    ul{
        list-style: none;
        @include center;
        li a {
            display:inline-block;
            padding: 1rem;
            text-decoration: none;
            font-size:13px;
        }
    }
    .linkContent-container{
        background-color: $primary;
        @include center;
        justify-content: space-between;
        padding: 20px;
    }
    .image{
        height: 70px;
        width: 70px;
        vertical-align: middle;
        padding: 10px;
    }

    .text-image{
        color: white;
        vertical-align: middle;
    }
    .jumbo{
        img{
            height: 400px;
            width: 100%;
        }
    }
    .row{
        display: flex;
    }
</style>
