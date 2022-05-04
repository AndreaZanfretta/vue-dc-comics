<template>
    <footer>
        <div class="footerNav">
            <div class="container">
                <div class="nav">
                    <div class="col">
                        <h3>DC Comics</h3>
                        <ul>
                            <li v-for="(link, index) in Comics" :key="index">{{link}}</li>
                        </ul>
                        <h3>Shop</h3>
                        <ul>
                            <li v-for="(link, index) in Shop" :key="index">{{link}}</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h3>DC</h3>
                        <ul>
                            <li v-for="(link, index) in DC" :key="index">{{link}}</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h3>Sites</h3>
                        <ul>
                            <li v-for="(link, index) in Sites" :key="index">{{link}}</li>
                        </ul>
                    </div>
                </div>
                <div class="logo"><img src="../assets/images/dc-logo-bg.png" alt=""></div>
            </div>
        </div>

        <div class="footerSocial">
            <div class="socialContainer">
                <div class="btn">
                    <a href="#"> Sign-up Now</a>
                </div>
                <div class="socials">
                    <h4>a</h4>
                    <p>a</p>
                    <p>a</p>
                    <p>a</p>
                    <p>a</p>
                    <p>a</p>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'AppFooter',
    data(){
        return{
            Comics: [
                "Characters",
                "Comics",
                "Movies",
                "Tv",
                "Games",
                "Videos",
                "News",
            ],
            Shop: [
                "Shop DC",
                "Shop DC Collectibles"
            ],
            DC: [
                "Terms Of Use",
                "Privacy policy(New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshop",
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                "Contact Us",
            ],
            Sites: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa",
            ],

        }
    },
}
</script>

<style scoped lang="scss">
@import '../styles/variables';
.footerNav{
    background-image: url('../assets/images/footer-bg.jpg');
    background-size: cover;
}
.container{
    width: 70%;
    height: 350px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    overflow: hidden;
}
.nav{
   display: flex;
}
ul{
    list-style: none;
    color: $grey;

        li{
            cursor: pointer;
            font-size: 14px;
            padding: 2px 0;
        }
}
.col{
    margin: 0 15px;
}
h3{
    color: $white;
    padding: 15px 0;
}
.footerSocial{
    background-color: $dark-grey;
    width: 100%;
    height: 130px;
}
.socialContainer{
    display: flex;
    width: 70%;
    margin: 0 auto;
    align-items: center;
    justify-content: space-between;
}
.btn{
    border: 3px solid $blue;
    padding: 10px 15px;

        a{
            text-decoration: none;
            color: $white;
        }
}
</style>