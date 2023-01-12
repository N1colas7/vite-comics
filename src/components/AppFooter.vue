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
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;
    
    .foot-sx{
        width: 50%;
    }
    .foot-dx{
        width: 50%;
        img{
            width: 50%;
            height: 100%;
            padding: 30px;
            position: relative;
            left: 100px;
        }
    }
    .container{
        background-image: url("/img/footer-bg.jpg");
        display: flex;
    }
    .col-footer{
        display: flex;
            h4{
                color: #fff;
            }
            ul{
                list-style: none;
                padding: 10px;
            li a{
                text-decoration: none;
                font-size:13px;
                color: #fff;
                opacity: 0.3;
                }
            }
    }
</style>
