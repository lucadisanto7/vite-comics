<script>
export default {
    data() {
        return {
            comics: [
                {
                    thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg/revision/latest?cb=20080809201655",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg/revision/latest/scale-to-width-down/1200?cb=20130627211607",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg/revision/latest?cb=20200929145132",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg/revision/latest?cb=20200929124651",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg/revision/latest?cb=20201123054610",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg/revision/latest?cb=20201124094800",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg/revision/latest?cb=20160303223223",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
        };
    }
}
</script>
<template>
    <main>
    <section class="text-white mt-4">
        <div class="jumbotron"></div>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    
                </div>
            </div>
        </div>
    </section>
    <section class="comics bg-dark text-white py-5">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h2 class="text-center mb-4 btn-primary label">CURRENT SERIES</h2>
                </div>
                <div class="col-md-2 col-sm-6 mb-4" v-for="comic in comics" :key="comic.series">
                    <div class=" text-white h-100">
                        <img :src="comic.thumb" class="card-img-top comic-img mt-4" :alt="comic.series">
                        <div class="card-body">
                            <h5 class="card-title">{{ comic.series }}</h5>
                        </div>
                    </div>
                </div>
                <div class="col-12 text-center">
                    <button class="btn btn-primary">Load More</button>
                </div>
            </div>
        </div>
    </section>
    <section class="bg-blue text-white py-5">
        <div class="container">
            <div class="row text-center">
                <div class="col d-flex align-items-center">
                    <img src="../assets/buy-comics-digital-comics.png" alt="Digital Comics" class="icon mb-2">
                    <h5>Digital Comics</h5>
                </div>
                <div class="col d-flex align-items-center">
                    <img src="../assets/buy-comics-merchandise.png" alt="DC Merchandise" class="icon mb-2">
                    <h5>DC Merchandise</h5>
                </div>
                <div class="col d-flex align-items-center">
                    <img src="../assets/buy-comics-subscriptions.png" alt="Subscription" class="icon mb-2">
                    <h5>Subscription</h5>
                </div>
                <div class="col d-flex align-items-center">
                    <img src="../assets/buy-comics-shop-locator.png" alt="Comic Shop Locator" class="icon-2 icon mb-2">
                    <h5>Comic Shop Locator</h5>
                </div>
                <div class="col d-flex align-items-center">
                    <img src="../assets/buy-dc-power-visa.svg" alt="DC Power Visa" class="icon mb-2">
                    <h5>DC Power Visa</h5>
                </div>
            </div>
        </div>
    </section>

    </main>
    
</template>
<style lang="scss">
.icon {
    width: 70px; 
    height: auto;
    display: block;
    margin: 0 auto 10px;  
}
.icon-2{
    width: 50px;
}

h5 {
    font-size: 20px;
    margin-left: 5px;  
}

.bg-blue{
    background-color: #0383f9;
}
.jumbotron{
    background: url('../assets/jumbotron.jpg') no-repeat;
    width: 100%;
    height: 500px; 
    background-size: cover;
    padding-bottom: 0px;
}
.bg-dark {
    background-color: #000;
}

.comics .card {
    background-color: transparent;
}

.comics .card-title {
    font-size: 18px;
    margin-top: 10px;
}

.comics .card-text {
    font-size: 14px;
    margin: 5px 0;
}

.btn-primary {
    background-color: #0383f9;
    border: none;
    padding: 10px 20px;
    font-size: 16px;
}
.comic-img{
    width: 200px;
    height: 200px;
}
.container{
    position: relative;
}
.label{
    position: absolute;
    width: 21%;
    top: -75px;
    font-size: 30px;
}
</style>