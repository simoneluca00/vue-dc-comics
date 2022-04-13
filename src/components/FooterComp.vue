<template>
  <div class="container">
      <div class="row">
            <div class="footerLists">
                <div class="col double-list">
                    <div>
                        <h2>dc comics</h2>
                        <ul>
                            <li v-for="(element,index) in dcComics" :key="index">
                                <a :href="`${element.url}`">
                                    {{element.name}}
                                </a>
                            </li>
                        </ul>
                    </div>

                    <div class="bottomList">
                        <h2>shop</h2>
                        <ul>
                            <li v-for="(element,index) in shop" :key="index">
                                <a :href="`${element.url}`">
                                    {{element.name}}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>   

                <div class="col central-list">
                        <h2>dc</h2>
                        <ul>
                            <li v-for="(element,index) in dcOptions" :key="index">
                                <a :href="`${element.url}`">
                                    {{element.name}}
                                </a>
                            </li>
                        </ul>
                </div>        

                <div class="col">
                    <h2>sites</h2>
                        <ul>
                            <li v-for="(element,index) in sites" :key="index">
                                <a :href="`${element.url}`">
                                    {{element.name}}
                                </a>
                            </li>
                        </ul>
                </div>           
            </div>

            <div class="logo-footer">
                <img src="../assets/img/dc-logo-bg.png" alt="logo DC footer">
            </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'FooterComp',

  data() {
      return {
          dcComics: [
            {
               name: 'Character',
               url: '/character'     
            },
            {
               name: 'Comics',
               url: '/comics'     
            },
            {
               name: 'Movies',
               url: '/movies'     
            },
            {
               name: 'TV',
               url: '/tv'     
            },
            {
               name: 'Games',
               url: '/games'     
            },
            {
               name: 'Videos',
               url: '/videos'     
            },
            {
               name: 'News',
               url: '/news'     
            },
            
          ],

          shop: [
            {
               name: 'Shop DC',
               url: '/shopDC'     
            },
            {
               name: 'Shop DC Collectibles',
               url: '/shopDC-Collectibles'     
            },
          ],

          dcOptions: [
            {
               name: 'Terms Of Use',
               url: '/termsOfUse'     
            },
            {
               name: 'Privacy policy',
               url: '/privacyPolicy'     
            },
            {
               name: 'Ad Choices',
               url: '/adChoices'     
            },
            {
               name: 'Advertising',
               url: '/advertising'     
            },
            {
               name: 'Jobs',
               url: '/jobs'     
            },
            {
               name: 'Subscriptions',
               url: '/subscriptions'     
            },
            {
               name: 'Talent Workshops',
               url: '/talentWorkshops'     
            },
            {
               name: 'CPSC Certificates',
               url: '/CPSCcertificates'     
            },
            {
               name: 'Ratings',
               url: '/Ratings'     
            },
            {
               name: 'Shop Help',
               url: '/shopHelp'     
            },
            {
               name: 'Contact Us',
               url: '/contactUs'     
            },
          ],

          sites: [
            {
               name: 'DC',
               url: '/DC'     
            },
            {
               name: 'MAD Magazine',
               url: '/MADMagazine'     
            },
            {
               name: 'DC Kids',
               url: '/DCKids'     
            },
            {
               name: 'DC Universe',
               url: '/DCUniverse'     
            },
            {
               name: 'DC Power Visa',
               url: '/DCPowerVisa'     
            },
          ]
        }
    }

}
</script>

<style scoped lang="scss">
@import '../style/variabili.scss';

@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');

.container {
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;

    .row {
        width: 85%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .footerLists {
            display: flex;
            color: $text-white;

            .col {
                display: flex;
                flex-direction: column;

                h2 {
                    text-transform: uppercase;
                    margin-bottom: 15px;
                    font-family: 'Bebas Neue', cursive;
                    font-size: 1.9em;
                    letter-spacing: 0.06em;
                }

                ul {
                    list-style-type: none;
                }

                li:not(li:last-child) {
                    margin-bottom: 5px;
                }

                a {
                    text-decoration: none;
                    color: $text-gray-footer;
                }
            }

            .double-list {
                display: flex;
                flex-direction: column;

                .bottomList {
                    margin-top: 30px;
                }
            }
            
            .central-list {
                margin: 0 50px;
            }
        }

        .logo-footer {
            margin: -70px 0;
        }
    }
}

</style>