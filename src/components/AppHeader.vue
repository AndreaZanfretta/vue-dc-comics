<template>
    <header>
        <div class="container">
            <div class="nav">
                <div class="logo"><img src="../assets/images/dc-logo.png" alt=""></div>
                <ul>
                    <li v-for="(section, index) in navSections" :key="index">
                        {{section.text}}
                        <div :class="{'active' : section.active}" class="act"></div>
                        </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    data(){
        return{
            navSections : [
                {
                    text: "Characters",
                    active: false,
                },
                {
                    text: "Comics",
                    active: true,
                },
                {
                    text: "Movies",
                    active: false,
                },
                {
                    text: "Tv",
                    active: false,
                },
                {
                    text: "Games",
                    active: false,
                },
                {
                    text: "Collectibles",
                    active: false,
                },
                {
                    text: "Videos",
                    active: false,
                },
                {
                    text: "Fans",
                    active: false,
                },
                {
                    text: "News",
                    active: false,
                },
                {
                    text: "Shop",
                    active: false,
                },
            ]
        }
    },
}
</script>

<style scoped lang="scss">
@import '../styles/variables';
.container{
    width: 70%;
    margin: 0 auto;
}
.nav{
    display: flex;
    align-items: center;
}
ul{
    list-style: none;
    width: 60%;
    
    li{
        display: inline-block;
        font-size: 18px;
        margin: 0 15px;
        position: relative;
    }
}
.logo{
    flex-grow: 1;
    height: 100%;
    img{
        padding: 10px;
    }
}
.act{
    position: absolute;
    bottom: -25px;
    left: 0;
    height: 5px;
    width: 100%;
    background-color: $blue;
    display: none;
}
.active{
    display: block;
}
</style>