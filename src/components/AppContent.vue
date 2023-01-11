<script>
    export default {
        data() {
            return {
                linkContent:[
                    {
                        label:'Digital Comics',
                        url: "../assets/vue-dc-comics-1/img/buy-comics-digital-comics.png"
                    },
                    {
                        label:'DC Merchandise',
                        url: "../assets/vue-dc-comics-1/img/buy-comics-merchandise.png"
                    },
                    {
                        label:'Susbscriptions',
                        url: "../assets/vue-dc-comics-1/img/buy-comics-subscriptions.png"
                    },
                    {
                        label:'Comic Shop Locator',
                        url: "../assets/vue-dc-comics-1/img/buy-comics-shop-locator.png"
                    },
                    {
                        label:'DC Power Visa',
                        url: "../assets/vue-dc-comics-1/img/buy-dc-power-visa.svg"
                    },
                ]
            }
        },
    }
</script>

<template>
    <div>
        <div class="contents-image">
            <h1> &lt;---- Contents goes here ----></h1>
        </div>
    </div>
    <div class="linkContent-container">
        <ul>
            <li v-for="(link, i) in linkContent" :key="i">
                    <img :src= "link.url" alt="image" >
                    <a :href= link.label>{{ link.label }}</a>
            </li>
        </ul>   
    </div>
</template>

<style lang="scss">
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    .contents-image{
        background-color: black;
        color:white;
        height: 100px;
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
    }
</style>
