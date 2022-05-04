<template>
    <main>


        <section id="black">
            <div class="content">
                <h2> --> Content Goes Here &lt;-- </h2>
            </div>
        </section>

        <section id="blue">
            <div class="container">
                <div class="card">
                    <img src="../assets/images/buy-comics-digital-comics.png" alt="">
                    <p>Digital Comics</p>
                </div>
                <div class="card">
                    <img src="../assets/images/buy-comics-merchandise.png" alt="">
                    <p>DC Merchandise</p>
                </div>
                <div class="card">
                    <img src="../assets/images/buy-comics-subscriptions.png" alt="">
                    <p>Subscriptions</p>
                </div>
                <div class="card">
                    <img src="../assets/images/buy-comics-shop-locator.png" alt="">
                    <p>Comic Shop Locator</p>
                </div>
                <div class="card">
                    <img src="../assets/images/buy-dc-power-visa.svg" alt="">
                    <p>DC Power Visa</p>
                </div>
            </div>
        </section>

    </main>
</template>

<script>
export default {
    name: 'AppMain',
    data(){
        return{

        }
    },
}
</script>

<style scoped lang="scss">
@import '../styles/variables';
#black{
    background-color: $black;
}
#blue{
    background-color: $blue;
}
.content{
    height: 150px;
    width: 70%;
    margin: 0 auto;
    color: $white;
    line-height: 150px;
    font-size: 20px;
}
.container{
    height: 180px;
    width: 65%;
    margin: 0 auto;
    color: $white;
    line-height: 180px;
    font-size: 18px;
    display: flex;
    align-content: center;
    justify-content: space-around;
    align-items: center;
}
.card{
    display: flex;
    align-items: center;
}
.card img{
    max-width: 60px;
    height: 60px;
    margin-right: 10px;
}
</style>