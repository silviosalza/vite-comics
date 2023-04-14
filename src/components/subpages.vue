<script>
export default {
    name: "subpages",
    data() {
        return {
            subpage: [
                {
                    text: "Digital Comics",
                    url: "#",
                    img: 'buy-comics-digital-comics.png'
                },
                {
                    text: "DC Merchandise",
                    url: "#",
                    img: 'buy-comics-merchandise.png'
                },
                {
                    text: "Subscription",
                    url: "#",
                    img: 'buy-comics-subscriptions.png'
                },
                {
                    text: "Comic Shop Locator",
                    url: "#",
                    img: 'buy-comics-shop-locator.png'
                },
                {
                    text: "DC Power Visa",
                    url: "#",
                    img: 'buy-dc-power-visa.svg'
                },
                
            ]
        }
    },
    methods:{
        ImgPath() {
            const imageUrl = new URL(`../assets/${this.subpage.img}`, import.meta.url).href;
            return imageUrl
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
    background-color: #0282F9;
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
        display: flex;
        padding-left: 0;

        li{
            list-style: none;
            padding: 0 2rem;
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
