<script>
export default{
    name: "comicCard",
    props:{
        img: String,
        name: String
    }
}

</script>

<template>
        <div class="card">
            <img class="frontpage" :src="img" alt="">
            <h4>{{name}}</h4>
        </div>
</template>



<style>
.card{
    width: calc(100%/6);
    padding: 1rem 0;
}

.frontpage{
    width: 230px;
    height: 230px;
    object-fit: cover;

}
</style>