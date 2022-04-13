<template>
  <div class="container">
      <div class="row">
        <div>
            <button id="btn-signUp">sign-up now!</button>
        </div>

        <div class="socialMedia">
            <h2>follow us</h2>

            <div class="iconSocial">
                <a href="/facebook">
                    <img src="../assets/img/footer-facebook.png" alt="Facebook icon">
                </a>

                <a href="/twitter">
                    <img src="../assets/img/footer-twitter.png" alt="Twitter icon">
                </a>

                <a href="/youtube">
                    <img src="../assets/img/footer-youtube.png" alt="Youtube icon"> 
                </a>

                <a href="/pinterest">
                    <img src="../assets/img/footer-pinterest.png" alt="Pinterest icon">
                </a>

                <a href="/periscope">
                    <img src="../assets/img/footer-periscope.png" alt="Periscope icon">
                </a>
            </div>

        </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'FooterBottomComp',

}
</script>

<style scoped lang="scss">
@import '../style/variabili.scss';

@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');


.container {
    background-color: $bg-gray-footerBottom;
    padding: 30px 0;
    position: relative;
    z-index: 1;

    .row {
        width: 85%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        #btn-signUp {
            background-color: transparent;
            border: 2px solid $active-blue;
            color: $text-white;
            padding: 10px;
            font-weight: bold;
            text-transform: uppercase;

            &:hover {
                opacity: 0.8;
                cursor: pointer;
            }
        }

        div.socialMedia {
            display: flex;
            align-items: center;

            h2 {
                font-family: 'Bebas Neue', cursive;
                color: $active-blue;
                text-transform: uppercase;
                margin-right: 30px;
            }

            .iconSocial {

                a {
                    margin: 0 10px;
                }
            }

        }
    }
}

</style>