<script>
export default {
    name: "headerDC",
    data() {
        return {
            links: [
                {
                    text: "Character",
                    url: "#",
                    current: false
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false
                },
                {
                    text: "TV",
                    url: "#",
                    current: false
                },
                {
                    text: "Games",
                    url: "#",
                    current: false
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false
                },
                {
                    text: "News",
                    url: "#",
                    current: false
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false
                },
            ]
        }
    }
}

</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="">
            </div>
            <nav class="nav-bar">
                <ul>
                    <li v-for="link in links" :class="link.current ? 'active' :''">
                        <a href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
  
</template>

<style scoped lang="scss">
header{
    height: 150px;
    width: 100%;
    display: flex;
.container{
    width: 1000px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

    ul{
        display: flex;
    }

    li{
        list-style: none;
    }
    a{
        text-decoration: none;
    }
}

</style>
