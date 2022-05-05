<template>
    <section id="cards-container">
        <div class="card">
            <img class="cover-image" :src="thumbs" :alt="series">
            <p class="title">{{series}}</p>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppCards',
    props: {
        thumbs: String,
        series: String,
    }
}
</script>

<style scoped lang="scss">
#cards-container{
    width: calc((100% / 6) - 20px);
    margin: 0 10px;
}
.card{
    width: 100%;
    height: 220px;
    margin: 20px 0;
    
}
.cover-image{
    width: 100%;
    height: 80%;
    display: block;
    object-fit: cover;
    object-position: top;
}
.title{
    line-height: 20px;
    padding-top: 20px;
}
</style>