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
            <img :src="img" alt="">
            <h3>{{name}}</h3>
        </div>
</template>



<style>
.row{
    background-color: black;
    color: white;
    display: flex;
    justify-content: space-around;
}


</style>