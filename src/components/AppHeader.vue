<script>
export default {
    data() {
        return {
            objs: [
                {
                    label: 'haracter',
                    link: '#',
                    acive: false
                },
                {
                    label: 'comics',
                    link: '#',
                    acive: false
                },
                {
                    label: 'movies',
                    link: '#',
                    acive: false
                },
                {
                    label: 'tv',
                    link: '#',
                    acive: false
                },
                {
                    label: 'games',
                    link: '#',
                    acive: false
                },
                {
                    label: 'collectibles',
                    link: '#',
                    acive: false
                },
                {
                    label: 'videos',
                    link: '#',
                    acive: false
                },
                {
                    label: 'fans',
                    link: '#',
                    acive: false
                },
                {
                    label: 'news',
                    link: '#',
                    acive: false
                },
                {
                    label: 'shop',
                    link: '#',
                    acive: false
                },

            ]
        }
    }
}
</script>

<template >
    <header>
        <div class="container">
            <div class="row d-flex space-between p-header">
                <div class="col-6">
                    <div class="img-container">
                        <img src="../../public/dc-logo.png" alt="Dc Logo">
                    </div>
                </div>
                <div class="col-6">
                    <ul class="uppercase d-flex space-between">
                        <li v-for="(obj, index) in objs" :key="index">
                            <a :href="obj.link">{{ obj.label }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="jumbotron">
            <div class="box-btn">
                <button class="btn">current series</button>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
li {
    margin-left: 20px;
    padding: 48px 0px;
}

a {
    font-weight: 500;
}

hr {
    margin-top: 50px;
}

li {}

li:hover {
    border-bottom: #0282F9 5px solid;

    a {
        color: #0282F9;
    }
}

.row {
    height: 120px;
}

.jumbotron {
    background-image: url(../assets/img/jumbotron.jpg);
    width: 100%;
    height: 500px;
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
}

.box-btn {
    position: absolute;
    bottom: -5%;
    left: 20%;
}

.btn {
    background-color: #0282F9;
    border: none;
    color: #fff;
    padding: 10px 40px;
    font-weight: 700;
    text-transform: uppercase;
    font-size: 1.2rem;
}
</style>