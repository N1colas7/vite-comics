<script>
    export default {

    }
</script>
<template>
    <div class="main-footer">
        <div class="container">
            <div class="foot-sx">
                <div class="col-footer">
                    <ul>
                        <li><h4>DC COMICS</h4></li>
                        <li><a href="#">Characters</a></li>   
                        <li><a href="#">Comics</a></li>   
                        <li><a href="#">Movies</a></li>   
                        <li><a href="#">TV</a></li>   
                        <li><a href="#">Games</a></li>   
                        <li><a href="#">Videos</a></li>   
                        <li><a href="#">News</a></li>   
                    </ul>
                    <ul>
                        <li><h4>SHOP</h4></li>
                        <li><a href="#">Shop DC</a></li>   
                        <li><a href="#">Shop DC Collectibles</a></li>     
                    </ul>
                    <ul>
                        <li><h4>DC</h4></li>
                        <li><a href="#">Term of Use</a></li>   
                        <li><a href="#">Privacy policy(New)</a></li>   
                        <li><a href="#">Ad Choices</a></li>   
                        <li><a href="#">Advertising</a></li>   
                        <li><a href="#">Jobs</a></li>   
                        <li><a href="#">Subscriptions</a></li>   
                        <li><a href="#">Talent Workshops</a></li>   
                        <li><a href="#">CPSC Certificates</a></li>   
                        <li><a href="#">Ratings</a></li>   
                        <li><a href="#">Shop Help</a></li>   
                        <li><a href="#">Contact Us</a></li>   
                    </ul>
                    <ul>
                        <li><h4>SITES</h4></li>
                        <li><a href="#">DC</a></li>   
                        <li><a href="#">Mad Magazine</a></li>     
                        <li><a href="#">DC Kids</a></li>   
                        <li><a href="#">DC Universe</a></li>     
                        <li><a href="#">DC Power Visa</a></li>     
                    </ul>
                </div>
            </div>
            <div class="foot-dx">
                <img src="/img/dc-logo-bg.png" alt="img">
            </div>    
        </div>        
    </div>
    <div class="end-foot">
        <div class="container-end">
            <div class="col-end">
                <h4 class="white-text">SING-UP NOW</h4>
            </div>
            <div class="col-end">
                <div class="follow-us">
                    <h4>FOLLOW US</h4>
                </div>
                <div class="social">
                    <img src="img/footer-facebook.png" alt="image">
                    <img src="img/footer-twitter.png" alt="image">
                    <img src="img/footer-youtube.png" alt="image">
                    <img src="img/footer-pinterest.png" alt="image">
                    <img src="img/footer-periscope.png" alt="image">
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;
    
    .foot-sx{
        width: 30%;
    }
    .foot-dx{
        width: 30%;
        img{
            width: 100%;
            height: 100%;
            position: relative;
            left: 30px;
        }
    }
    .container{
        background-image: url("/img/footer-bg.jpg");
        display: flex;
    }
    .col-footer{
        @include center;
        margin: 2rem 1rem;
        display: flex;
            h4{
                color: #fff;
            }
            ul{
                list-style: none;
                padding: 10px;
                flex-wrap: wrap;
            li a{
                text-decoration: none;
                font-size:13px;
                color: #fff;
                opacity: 0.3;
                }
            }
    }
    .container-end{
        @include center;
        background-color: rgb(51, 50, 50);
        justify-content: space-around;
            .col-end{
                margin: 1rem 1rem;
                display: flex;
                 .white-text{
                    color: #fff;
                    opacity: 0.8;
                    border: 2px solid $primary;
                    padding: 15px;
                 }
                 .follow-us{
                    padding: 15px;
                    color: $primary;
                 }
                 img{
                    padding: 5px;
                 }

            }
    }
</style>
