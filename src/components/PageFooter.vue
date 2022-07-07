<template>

  <div class="total-footer">

    <!-- Top part of the footer - sites links and faq -->
    <div class="top-footer">
        <div class="container">

            <div class="faq-cols">

                <!-- Dc comics list -->
                <ul>
                    <li>
                        <h3>DC COMICS</h3>
                    </li>
                    <li>
                        <a href="#">Characters</a>
                    </li>
                    <li>
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">Games</a>
                    </li>
                    <li>
                        <a href="#">Videos</a>
                    </li>
                    <li>
                        <a href="#">News</a>
                    </li>

                    <!-- Shop list -->
                    <ul class="sub-list">
                        <li>
                            <h3>SHOP</h3>
                        </li>
                        <li>
                            <a href="#">Shop DC</a>
                        </li>
                        <li>
                            <a href="#">Shop DC Collectibles</a>
                        </li>
                    </ul>
                </ul>

                <!-- Dc faq list -->
                 <ul>
                    <li>
                        <h3>DC</h3>
                    </li>
                    <li>
                        <a href="#">Terms of use</a>
                    </li>
                    <li>
                        <a href="#">Privacy policy (new)</a>
                    </li>
                    <li>
                        <a href="#">Ad choices</a>
                    </li>
                    <li>
                        <a href="#">Advertising</a>
                    </li>
                    <li>
                        <a href="#">Jobs</a>
                    </li>
                    <li>
                        <a href="#">Subscriptions</a>
                    </li>
                    <li>
                        <a href="#">Talent workshops</a>
                    </li>
                    <li>
                        <a href="#">CPSC certificates</a>
                    </li>
                    <li>
                        <a href="#">Ratings</a>
                    </li>
                    <li>
                        <a href="#">Shop help</a>
                    </li>
                    <li>
                        <a href="#">Contact us</a>
                    </li>
                </ul>

                <!-- Sites links -->
                <ul>
                     <li>
                        <h3>SITES</h3>
                    </li>
                    <li>
                        <a href="#">DC</a>
                    </li>
                    <li>
                        <a href="#">MAD magazine</a>
                    </li>
                    <li>
                        <a href="#">DC kids</a>
                    </li>
                    <li>
                        <a href="#">DC universe</a>
                    </li>
                    <li>
                        <a href="#">DC power visa</a>
                    </li>
                </ul>
            </div>

            <div>
                <img class="footer-logo" src="../assets/img/dc-logo-bg.png" alt="dc logo footer">
            </div>
        </div>
        
    </div>

    <!-- Bottom section of the footer - social media and sign up button -->
    <div class="bottom-footer">
        <div class="container">

            <!-- Sign up button -->
            <div class="button-sign-up">
                <div href="#">SIGN UP NOW! </div>
            </div>

            <!-- Social media area -->
            <div class="social-area">
                <span>FOLLOW US</span>

                <ul class="social-list">
                    <li>
                        <img src="../assets/img/footer-facebook.png" alt="dc social media">
                    </li>
                    <li>
                        <img src="../assets/img/footer-twitter.png" alt="dc social media">
                    </li>
                    <li>
                        <img src="../assets/img/footer-youtube.png" alt="dc social media">
                    </li>
                    <li>
                        <img src="../assets/img/footer-pinterest.png" alt="dc social media">
                    </li>
                    <li>
                        <img src="../assets/img/footer-periscope.png" alt="dc social media">
                    </li>
                </ul>
            </div>
        </div>
    </div>
  </div>

</template>

<script>

  export default {
    name: "PageFooter"
  }

</script>

<style lang="scss" scoped>

    @import "../style/brand-colors.scss";

    .total-footer {
        // Top part of the footer styles
        .faq-cols {
            display: flex;
            align-self: center;
            ul {
                margin: 0 30px;
                .sub-list {
                    margin: 0;
                }
                li {
                    margin: 6px;
                }
                a {
                    color: $tertiary-color;
                }
            }
        }
        .container {
            display: flex;
            justify-content: space-between;
        }
        .top-footer {
            display: flex;
            height: 400px;
            background-image: url('../assets/img/footer-bg.jpg');
            background-size: cover;
            h3 {
                color: $secondary-color;
                margin: 10px 0;
            }
            .footer-logo {
                width: 550px;
                position: relative;
                right: 0;
                bottom: 50px;
            }
        }
        // Bottom part of the footer styles
        .bottom-footer {
            position: relative;
            background-color: #303030;
            height: 140px;
            .container {
                height: 100%;
                display: flex;
                align-items: center;
                h3 {
                    color: $secondary-color;
                }
                .button-sign-up {
                    color: $secondary-color;
                    border: 2px solid $primary-color;
                    padding: 15px;
                    font-weight: 700;
                    cursor: pointer;
                    font-size: 20px;
                }
                .social-area {
                    display: flex;
                    align-items: center;
                }
                span {
                    color: $primary-color;
                    font-size: 20px;
                    font-weight: 700;
                    }
                .social-list {
                    display: flex;
                    margin-left: 20px;
                    li {
                        margin-left: 10px;
                        cursor: pointer;
                    }
                }
            }
        }
    }

</style>
