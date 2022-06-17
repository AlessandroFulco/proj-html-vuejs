<template>
    <header>
        <img :src="logo" :alt="myName">
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
        color: #fff;
        width: 100%;
        height: 100px;
        background-color: #000;
        position: fixed;
        top: 0;
        left: 0;
    }
</style>