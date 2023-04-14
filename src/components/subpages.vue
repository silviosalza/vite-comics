<script>
export default {
    name: "subpages",
    data() {
        return {
            subpage: [
                {
                    text: "Digital Comics",
                    url: "#",
                    img: '../assets/buy-comics-digital-comics.png'
                },
                {
                    text: "DC Merchandise",
                    url: "#",
                    img: '../assets/buy-comics-merchandise.png'
                },
                {
                    text: "Subscription",
                    url: "#",
                    img: '../assets/buy-comics-subscriptions.png'
                },
                {
                    text: "Comic Shop Locator",
                    url: "#",
                    img: '../assets/buy-comics-shop-locator.png'
                },
                {
                    text: "DC Power Visa",
                    url: "#",
                    img: '../assets/buy-dc-power-visa.svg'
                },
                
            ]
        }
    }
}

</script>

<template>
    <section class="subpages">
        <div class="container">
            <ul>
                <li v-for="(element,index) in subpage" :key="index">
                    <a href="">{{ element.text.toUpperCase() }}</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<style scoped lang="scss">
.subpages{
    background-color: blue;
    color: white;
    height: 150px;
    .container{
        max-width: 1500px;
        height: 150px;
        margin: 0 auto; 
        display: flex;
        align-items: center;  
    }

    ul{
        width: 100%;
        display: flex;
        justify-content: space-between;

        li{
            list-style: none;
            a{
                color: inherit;
                text-decoration: none;
            }
            img{
                width: 100%;
            }
        }
    }
}
</style>
