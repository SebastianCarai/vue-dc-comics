<template>
    <header>
        <div class="container_70">
            <img src="../assets/img/dc-logo.png" alt="DC Logo">
            <ul>
                <li v-for="(element,index) in headerLinks" :key="index" class="header_li" :class="{active: element.headerActive}">
                    <a :href="element.url"> {{ element.text }} </a>
                </li>
            </ul>
        </div>
    </header>
</template>

<script>
export default{
    name:"Header",
    data: function(){
        return{
            headerLinks:[
                {
                    text:'CHARACTERS',
                    url: '#',
                    headerActive: false
                },
                {
                    text:'COMICS',
                    url: '#',
                    headerActive: true
                },
                {
                    text:'MOVIES',
                    url: '#',
                    headerActive: false
                },
                {
                    text:'TV',
                    url: '#',
                    headerActive: false
                },
                {
                    text:'GAMES',
                    url: '#',
                    headerActive: false
                },
                {
                    text:'COLLECTIBLES',
                    url: '#',
                    headerActive: false
                },
                {
                    text:'VIDEOS',
                    url: '#',
                    headerActive: false
                },
                {
                    text:'FANS',
                    url: '#',
                    headerActive: false
                },
                {
                    text:'NEWS',
                    url: '#',
                    headerActive: false
                },
                {
                    text:'SHOP',
                    url: '#',
                    headerActive: false
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';
header{
    div{
        height: $header_height;
        line-height: $header_height;
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: $header_height;
    }
    img{
        height: 70px;
        width: auto;
    }
    .header_li{
        display: inline-block;
        padding: 0 15px;
        font-size: 14px;
        font-weight: 700;
        a{
            display: inline-block;
            line-height: 100px;
        }
        &:hover{
            a{
                border-bottom: 6px solid $main_color;
                color: $main_color;   
            }
        }
    }
    .header_li.active{
        a{
            border-bottom: 6px solid $main_color;
            color: $main_color;
        }
    }
}
</style>
