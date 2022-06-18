<template>
    <footer>
        <div class="containerFooter">
            <div id="call">
                CALL OUR EXPERT TODAY 1.800.555.6789
            </div>
            <div>
                <div class="copy">
                    <div>&copy; Copyright 2012 - 2020 |</div>
                    <div v-for="(item, index) in link" :key="index" >{{item.nameLink}} |</div>
                    

                </div>
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
        <div id="arrow-up-icon">
            <i class="arrow"><font-awesome-icon icon="fa-solid fa-angle-up" /></i>
        </div>
    </footer>
</template>

<script>

export default {
    name: "MyFooter",
    data() {
        return {
            link: [
                {
                    nameLink: "Avada Theme by Theme Fusion"
                },
                {
                    nameLink: "All Rights Reserved"
                },
                {
                    nameLink: "Powered by WordPress"
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../../public/scss/icon-fontAwesome.scss';
    footer {
        position: relative;
        
        .containerFooter {
            
            height: 200px;
            width: 70%;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            justify-content: center;
            gap: 40px;
            
            #call {
                font-weight: bold;
            }


            div {
                display: flex;
                justify-content: space-between;
                .copy {
                    display: flex;
                    color: #666;
                    font-size: 14px;
                    
                    div {
                        margin-right: 10px;
                    }
                }
            }
        }
    }
</style>