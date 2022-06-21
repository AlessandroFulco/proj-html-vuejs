<template>
    <div>
        <div class="container-preHeader">
            <div id="preHeader">
            <p>
                Avada & Associates legal team announce deal to open up oil & gas
            </p>
            <div>
                <!-- icone fontawesome social -->
                <a href="#">
                    <i><font-awesome-icon icon="fa-brands fa-facebook-square" /></i>
                </a>
                <a href="#">
                    <i><font-awesome-icon icon="fa-brands fa-twitter-square" /></i>
                </a>
                <a href="#">
                    <i><font-awesome-icon icon="fa-brands fa-instagram-square" /></i>
                </a>
                <a href="#">
                    <i><font-awesome-icon icon="fa-brands fa-youtube-square" /></i>
                </a>
            </div>
        </div>
        </div>

        <!-- header -->
        <header>
            <div class="container">
                <img :src="logo" :alt="myName">

                <!-- menu nav -->
                <nav>
                    <ul>
                        <li v-for="(item, index) in menu" :key="index">
                            <a href="#" @click.prevent="changeActive(item)" :class="item.active ? 'here' : '' ">{{item.title}}</a>
                        </li>
                    </ul>
                </nav>  
            </div>
        </header>
    </div>
</template>

<script>

export default {
    name: "MyHeader",
    data() {
        return {
            myName: "Avada Law",
            logo: require('../assets/images/avada-law-logo.png'),
            menu: [
                {
                    title: "Home",
                    active: true
                },
                {
                    title: "Who We Are",
                    active: false
                },
                {
                    title: "What We Do",
                    active: false
                },
                {
                    title: "Where We Work",
                    active: false
                },
                {
                    title: "Careers",
                    active: false
                },
                {
                    title: "News",
                    active: false
                },
                {
                    title: "Contact",
                    active: false
                }
            ]
        }
    },
    methods: {
        changeActive(item) {
            this.menu.forEach(element => {
                element.active = false;
            });
            item.active = true;
        },
    }
}
</script>

<style scoped lang="scss">
@import '../../public/scss/icon-fontAwesome.scss';
@import '../../public/scss/color-variable.scss';
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

    .container-preHeader {
        background-color: #eee;
        #preHeader {
            width: 70%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 5px;
        p {
            font-size: 12px;
            color: #666;
        }
        
    }
    }
    header {
        width: 100%;
        background-color: #fff;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 70%;
            margin: 0 auto;
            height: 80px;
            nav {
                ul {
                    list-style-type: none;
                    display: flex;
                    align-items: center;
                    
                    li {
                        height: 80px;
                        margin-right: 20px;
                        display: flex;
                        a {
                            font-size: 14px;
                            text-decoration: none;
                            color: #666;
                            font-weight: bold;
                            height: 80px;
                            line-height: 80px;
                            vertical-align: middle;

                            
                        }
                        a.here {
                            color: $link-active;
                            border-top: 2px solid $link-active;
                            line-height: 75px;
                        }
                    }
                }
            }
        }
    }
</style>