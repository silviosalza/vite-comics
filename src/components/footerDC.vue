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
                <div>
                    <h3>DC COMICS</h3>
                    <ul v-for="(element,index) in ComicLink">
                        <li>{{element}}</li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul v-for="(element,index) in ShopLink">
                        <li>{{element}}</li>
                    </ul>
                </div>
                <div>
                    <h3>DC</h3>
                    <ul v-for="(element,index) in DCLink">
                        <li>{{element}}</li>
                    </ul>
                </div>
                <div>
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
.container{
    max-width: 1000px;
    margin: 0 auto;
    display: flex;
}
.footer-links{
    display: flex;
    div{
    }
    li{
        font-size: 1rem;
        list-style: none;
        
    }
}



</style>
