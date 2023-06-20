<script>
    export default {
        data(){
            return{
                objs : [
                    {
                        label: 'Character',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Comics',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Movies',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Tv',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Games',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Collectibles',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Videos',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Fans',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'News',
                        link: '#',
                        acive: false
                    },

                ],

                list:[
                    {
                        label: 'Shop DC',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Shop DC Collectibles',
                        link: '#',
                        acive: false
                    },
                ],
                
                dc: [
                    {
                        label: 'Term of Use',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Pravacy policy (New)',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Ad Choices',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Advertising',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Jobs',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Subscriptions',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Talent Workshops',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'CPSC Certificates',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Ratings',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Shop Help',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'Contact us',
                        link: '#',
                        acive: false
                    },
                
                ],

                sites: [
                    {
                        label: 'DC',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'MAD Magazine',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'DC Kids',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'DC Universe',
                        link: '#',
                        acive: false
                    },
                    {
                        label: 'DC Power Visa',
                        link: '#',
                        acive: false
                    },

                ]
            }
        }
    }
</script>

<template >
    <div>
        <div class="jumbotron">
            <div class="container">
                <div class="row d-flex">
                    <div class="col-6 d-flex mt">
                        <div class="footer-one">
                            <ul> <h2 class="uppercase">dc comics</h2>
                                <li v-for="(obj, index) in objs" :key="index">
                                    <a :href="obj.link" >{{ obj.label }}</a>
                                </li>
                            </ul>
                            
                            <ul class="lil"><h2 class="uppercase">shop</h2>
                                <li v-for="(obj, index) in list" :key="index">
                                    <a :href="obj.link" >{{ obj.label }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="footer-two">
                            <ul><h2 class="uppercase">dc</h2>
                                <li v-for="(obj, index) in dc" :key="index">
                                    <a :href="obj.link" >{{ obj.label }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="footer-three">
                            <ul><h2 class="uppercase">dc</h2>
                                <li v-for="(obj, index) in sites" :key="index">
                                    <a :href="obj.link" >{{ obj.label }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-6">
                        <div class="img-container">
                            <img src="../assets/img/dc-logo-bg.png" alt="">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .jumbotron{
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        
    }

    h2{
        margin-bottom: 10px;
        color: #fff;
    }

    li{
        margin-bottom: 5px;
    }

    a{
        color: #959595;
    }

    a:hover{
        color: #fff;
    }

    .lil{
        margin-top: 30px;
    }

    .footer-three, .footer-two{
        margin-left: 50px;
    }

    .mt{
        margin-top: 50px;
    }
</style>