<script>
import AppCard from './AppCard.vue'
export default {
    components: {
        AppCard
    },

    data() {
        return {
            lists: [
                {
                    immg: './src/assets/img/buy-comics-digital-comics.png',
                    lable: 'digital comics'
                },
                {
                    immg: './src/assets/img/buy-comics-merchandise.png',
                    lable: 'dc merchandise'
                },
                {
                    immg: './src/assets/img/buy-comics-subscriptions.png',
                    lable: 'subscription'
                },
                {
                    immg: './src/assets/img/buy-comics-shop-locator.png',
                    lable: 'comic shop locator'
                },
                {
                    immg: './src/assets/img/buy-dc-power-visa.svg',
                    lable: 'dc power visa'
                }
            ],

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
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
        }
    }
}
</script>

<template >
    <div>
        <div class="jumbotron-black">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div class="card-container d-flex flex-wrap">
                            <AppCard v-for="(comic, index) in comics" :key="index" :comicsEdition="comic" />
                        </div>
                    </div>
                    <div class="col-button ">
                        <button class="btn">load more</button>
                    </div>
                </div>
            </div>
        </div>
        <div class="jumbotron-blue">
            <div class="container container-blue">
                <div class="content">
                    <ul class="d-flex">
                        <li :key="index" v-for="(list, index) in lists" class="d-flex align-center">
                            <div class="img-container">
                                <img :src="list.immg" :alt="list.lable">
                            </div>
                            <h4 class="uppercase">{{ list.lable }}</h4>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.jumbotron-black {
    background-color: #1C1C1C;
}

.main-content {
    color: #fff;
    padding: 50px 0px;
}

.jumbotron-blue {
    background-color: #0282F9;
    padding: 50px 0px;
}

.img-container {
    width: 20%;
}

h4 {
    margin-left: 10px;
    color: #fff;
    font-weight: 400;
}

.container-blue {
    max-width: 1170px;
}

.flex-wrap {
    flex-wrap: wrap;
    align-items: center;
}

.col-button {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 40px 0px;
}

.btn {
    padding: 10px 35px;
    background-color: #0282F9;
    border: none;
    text-transform: uppercase;
    font-weight: 600;
    color: #fff;
}
</style>