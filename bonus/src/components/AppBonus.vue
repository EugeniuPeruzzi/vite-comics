<script>
    export default {
        data(){
            return{
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
                ]
            }
        }
    }
</script>

<template>
    <div>
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
        .jumbotron-blue{
        background-color: #0282F9;
        padding: 50px 0px;
    }
    
    .img-container{
        width: 20%;
    }


    h4{
        margin-left: 10px;
        color: #fff;
        font-weight: 400;
    }

    .container-blue{
        max-width: 1170px;
    }

</style>