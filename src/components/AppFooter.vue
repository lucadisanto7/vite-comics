<script>
export default {
    
}
</script>
<template>
    <div>
        <body>       
            <div class="footer-bg">
                <div class="bg-dc d-flex justify-content-center align-items-center">
                    <img src="../assets/dc-logo-bg.png" alt="DC Logo">
                </div>
                <div class="container">
                    <div class="row footer-links">
                        <div class="col-md-2 mb-4 mt-4">
                            <h5>DC COMICS</h5>
                            <ul class="list-unstyled">
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Comics</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">TV</a></li>
                                <li><a href="#">Games</a></li>
                                <li><a href="#">Videos</a></li>
                                <li><a href="#">News</a></li>
                            </ul>
                            <h5>SHOP</h5>
                            <ul class="list-unstyled">
                              <li><a href="#">Shop DC</a></li>
                              <li><a href="#">Shop DC Collectibles</a></li>
                            </ul>
                        </div>
                        <div class="col-md-2 mt-4">
                            <h5>DC</h5>
                            <ul class="list-unstyled">
                                <li><a href="#">Terms Of Use</a></li>
                                <li><a href="#">Privacy policy (New)</a></li>
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
                        </div>
                        <div class="col-md-2 mt-4">
                            <h5>SITES</h5>
                            <ul class="list-unstyled">
                                <li><a href="#">DC</a></li>
                                <li><a href="#">MAD Magazine</a></li>
                                <li><a href="#">DC Kids</a></li>
                                <li><a href="#">DC Universe</a></li>
                                <li><a href="#">DC Power Visa</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </body>
        <footer class="footer d-flex justify-content-between align-items-center">
            <div class="ml-4 container">
                <button class="btn btn-outline-primary white">SIGN-UP NOW!</button>
            </div>
            <div class="d-flex align-items-center">
                <span class="mr-3">FOLLOW US</span>
                <div class="social-icons">
                    <a href="#"><img src="../assets/footer-facebook.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-periscope.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-pinterest.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-twitter.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-youtube.png" alt=""></a>
                </div>
            </div>
        </footer>
    </div>
</template>
<style lang="scss">
@use '../styles/partials/generals.scss';
.bg-dc {
    background: url('../assets/dc-logo-bg.png') no-repeat center center;
    background-size: cover;
    position: absolute;
    right: 250px;
    height: 450px;
    opacity: 0.5;
    z-index: 0;
}
.footer-bg {
    background: url('../assets/footer-bg.jpg') no-repeat center center;
    background-size: cover;
    position: relative;
    z-index: -1;
}
.footer-links {
    color: white;
    padding: 20px 0;
    position: relative;
    z-index: 2;
}
.footer-links ul {
    padding: 0;
    list-style-type: none;
}

.footer-links a {
    color: #929492;
    text-decoration: none;
    display: block;
    padding: 2px 0;
}

.footer-links a:hover {
    text-decoration: underline;
    color: white;
}
.footer {
    background-color: #333;
    color: #fff;
    padding: 10px 0;
    z-index: 2;
    padding: 20px;
}
.footer a {
    color: #00f;
    text-decoration: none;
}
.footer a:hover {
    text-decoration: underline;
}
.social-icons a {
    color: #999;
    font-size: 24px;
    margin: 0px 10px;
}
.social-icons a:hover {
    color: #fff;
}
.white{
    color: white;
}
.btn{
    padding: 15px;
}
</style>