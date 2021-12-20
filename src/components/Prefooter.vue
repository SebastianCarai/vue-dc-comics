<template>
    <section>
        <div class="container_70">
            <ul>
                <li v-for="(element, index) in prefooterArray" :key="index">
                    <img :src="require('../assets/img/' + element.path)" alt="" class="prefooter_img"> 
                    <a :href="element.url">{{ element.text }}</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default{
    name: "Prefooter",
    data: function(){
        return{
            prefooterArray: [
                {
                    text: 'DIGITAL COMICS',
                    path: 'buy-comics-digital-comics.png',
                    url: '#'
                },
                {
                    text: 'DC MERCHANDISE',
                    path: 'buy-comics-merchandise.png',
                    url: '#'
                },
                {
                    text: 'SUBSCRIPTION',
                    path: 'buy-comics-subscriptions.png',
                    url: '#'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    path: 'buy-comics-shop-locator.png',
                    url: '#'
                },
                {
                    text: 'DC POWER VISA',
                    path: 'buy-dc-power-visa.svg',
                    url: '#'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';
section {
    background-color: $main_color;
    padding: 50px 0;
    color: $secondary_color;
    li{
    display: inline-block;
    margin: 0 30px;
        .prefooter_img{
            width: 50px;
            display: inline-block;
            vertical-align: middle;
            margin: 0 10px;
        }
    }
}
</style>