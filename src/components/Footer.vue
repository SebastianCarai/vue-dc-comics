<template>
    <section>
        <div class="container_70">
            <div class="footer_left_col">
                        
                <div>
                    <h3>DC Comics</h3>
                    <ul>
                        <li v-for="(element, index) in footerDcComics" :key="index">
                            <a :href="element.url" class="footer_link"> {{ element.text }} </a>
                        </li>
                    </ul>

                    <h3>SHOP</h3>
                    <ul>
                        <li v-for="(element, index) in footerShop" :key="index">
                            <a :href="element.url" class="footer_link"> {{ element.text }} </a>
                        </li>
                    </ul>
                </div>

                <div>
                    <h3>DC</h3>
                    <ul>
                        <li v-for="(element, index) in footerDC" :key="index">
                            <a :href="element.url" class="footer_link"> {{ element.text }} </a>
                        </li>
                    </ul>
                </div>

                <div>
                    <h3>DC</h3>
                    <ul>
                        <li v-for="(element, index) in footerSites" :key="index">
                            <a :href="element.url" class="footer_link"> {{ element.text }} </a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="footer_right_col"></div>
        </div>
    </section>
</template>

<script>
export default{
    name:"Footer",
    data: function() {
        return{
            footerDcComics: [
                {
                    text: 'Characters',
                    url: '#'
                },
                {
                    text: 'Comics',
                    url: '#'
                },
                {
                    text: 'Movies',
                    url: '#'
                },
                {
                    text: 'TV',
                    url: '#'
                },
                {
                    text: 'Games',
                    url: '#'
                },
                {
                    text: 'Videos',
                    url: '#'
                },
                {
                    text: 'News',
                    url: '#'
                }
            ],
            footerShop: [
                {
                    text: 'Shop DC',
                    url: '#'
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#'
                }
            ],
            footerDC: [
                {
                    text: 'Terms Of Use',
                    url: '#'
                },
                {
                    text: 'Privacy policy (New9',
                    url: '#'
                },
                {
                    text: 'Ad Choices',
                    url: '#'
                },
                {
                    text: 'Advertising',
                    url: '#'
                },
                {
                    text: 'Jobs',
                    url: '#'
                },
                {
                    text: 'Subscriptions',
                    url: '#'
                },
                {
                    text: 'Talent Workshops',
                    url: '#'
                },
                {
                    text: 'CPSC Certificates',
                    url: '#'
                },
                {
                    text: 'Ratings',
                    url: '#'
                },
                {
                    text: 'Shop Help',
                    url: '#'
                },
                {
                    text: 'Contact Us',
                    url: '#'
                }
            ],
            footerSites: [
                {
                    text: 'DC',
                    url: '#'
                },
                {
                    text: 'DC Kids',
                    url: '#'
                },
                {
                    text: 'DC Universe',
                    url: '#'
                },
                {
                    text: 'DC Power Visa',
                    url: '#'
                }
            ]
            
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
section{
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    div.container_70{
        display: flex;
    }
    .footer_left_col{
        color: $secondary_color;
        display: flex;
        padding: 30px 0 50px;
        width: 40%;
        div{
            margin-right: 30px;
        }

        h3{
            margin-top: 15px;
        }
        li{
            margin: 5px 0;
            .footer_link{
                color: gray;
                font-size: 13px;
            }
            &:hover{
                text-decoration: underline;
            }
        }
    }
    .footer_right_col{
        width: 60%;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: center;
    }
}
</style>