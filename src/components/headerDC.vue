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
                        <a href="link.url">{{ link.text.toUpperCase() }}</a>
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
    border-top: 20px solid black;
    
.container{
    width: 1500px;
    height: 100%;
    margin: 0 auto;
    display: flex;
    align-items: center
}

    ul{
        display: flex;
        padding: 0;
    }

    li{
        list-style: none;
        padding-right:  1rem;
    }
    a{
        text-decoration: none;
        color: black;
        font-weight: 700;
        &:hover{
            color: #0282F9;
        }
    }
}

</style>
