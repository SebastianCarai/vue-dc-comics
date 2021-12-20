<template>
    <section>
        <div class="container_70">
            <div>
                <a href="#" class="signup_btn">SIGN UP NOW</a>
            </div>
            <ul>
                <li class="social_text">FOLLOW US</li>
                <li v-for="(element,index) in socialLogos" :key="index">
                    <img :src="require('../assets/img/' +element)" alt="">
                </li>
            </ul>
        </div>
    </section>
</template>

<script lang="ts">
export default{
    name:"References",
    data: function(){
        return{
            socialLogos:[
                'footer-facebook.png',
                'footer-periscope.png',
                'footer-pinterest.png',
                'footer-twitter.png',
                'footer-youtube.png', 
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
section{
    background-color:#303030;
    padding: 50px 0;
    div.container_70{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
        .signup_btn{
            color: white;
            padding: 15px;
            border: 3px solid $main_color;
        }
        li{
            display: inline-block;
            vertical-align: middle;
            margin: 0 10px;
            &.social_text{
                color: $main_color;
                font-weight: 700;
                font-size: 25px;
            }
        }
}

</style>
