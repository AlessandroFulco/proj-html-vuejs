<template>
    <header>
        <div class="container">
            <img :src="logo" :alt="myName">
            <nav>
                <ul>
                    <li v-for="(item, index) in menu" :key="index">
                        <a href="#">{{item.title}}</a>
                    </li>
                </ul>
            </nav>  
        </div>
    </header>
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
                    title: "Home"
                },
                {
                    title: "Who We Are"
                },
                {
                    title: "What We Do"
                },
                {
                    title: "Where We Work"
                },
                {
                    title: "Careers"
                },
                {
                    title: "News"
                },
                {
                    title: "Contact"
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
    header {
        width: 100%;
        background-color: #fff;
        position: fixed;
        top: 0;
        left: 0;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 70%;
            margin: 0 auto;
            height: 100px;
            nav {
                ul {
                    list-style-type: none;
                    li {
                        display: inline-block;
                        margin-right: 10px;
                        
                        a {
                            font-size: 14px;
                            text-decoration: none;
                            color: #666;
                            font-weight: bold;
                            padding: 10px;

                            &:hover {
                                background-color: #ddd;
                                color: #000;
                            }
                        }
                    }
                }
            }
        }
    }
</style>