<script>
export default {
    name: "footerDC",
    data() {
        return {
            ComicLink: ["Character", "Comics", "Movies", "TV", "Games", "Videos", "News"],
            ShopLink: ["Shod DC", "Shop DC Collectilbles"],
            DCLink: ["Terms Of Use", "Privacy Policy", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshop", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
            SitesLink:["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]

        }
    }
}
</script>

<template>
    <section class="footerDC">
        <div class="container">
            <div class="footer-links">
                <div class="list">
                    <h3>DC COMICS</h3>
                    <ul v-for="(element,index) in ComicLink">
                        <li>{{element}}</li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul v-for="(element,index) in ShopLink">
                        <li>{{element}}</li>
                    </ul>
                </div>
                <div class="list">
                    <h3>DC</h3>
                    <ul v-for="(element,index) in DCLink">
                        <li>{{element}}</li>
                    </ul>
                </div>
                <div class="list">
                    <h3>SITES</h3>
                    <ul v-for="(element,index) in SitesLink">
                        <li>{{element}}</li>
                    </ul>
                </div>
            </div>
            <img src="../assets/dc-logo-bg.png" alt="">
        </div>
    </section>
  
</template>

<style scoped lang="scss">
.footerDC{
    background-image: url(../assets/footer-bg.jpg);
}
.container{
    max-width: 1500px;
    margin: 0 auto;
    display: flex;
}
.footer-links{
    display: flex;
    .list{
        padding: 0 1rem;
    }
    .list h3{
        padding: 1.5rem 0;
    }
    h3{
        color: white
    }
    ul{
        padding-left: 0;
    }
    li{
        font-size: 1rem;
        color: rgb(164, 164, 164);
        list-style: none;  
        padding-left: 0;
        padding: 0.2rem 0;
    }
}
img{
    width: 30%;
}

</style>
