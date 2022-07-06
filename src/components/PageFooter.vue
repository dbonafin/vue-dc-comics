<template>

  <div class="total-footer">

    <div class="top-footer">
        
        <div class="container">

            <div>
                <h3>Links</h3>
            </div>

            <div>
                <img class="footer-logo" src="../assets/img/dc-logo-bg.png" alt="dc logo footer">
            </div>
        </div>
        
    </div>

    <div class="bottom-footer">
        <div class="container">
           <h3>bottom footer here</h3>
        </div>
    </div>
  </div>

</template>

<script>

  export default {
    name: "PageFooter"
  }

</script>

<style lang="scss">

    @import "../style/brand-colors.scss";

    .total-footer {

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
            }
            .footer-logo {
                width: 460px;
            }
        }
        .bottom-footer {
            position: relative;
            background-color: #303030;
            // test
            height: 200px;
            line-height: 200px;
            h3 {
                color: $secondary-color;
            }
        }
    }

</style>
