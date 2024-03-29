<script setup>
import Links from "./components/Links.vue"
import { profileData } from "./data.js"

const image = profileData.image
</script>

<template>
    <div class="container">
        <img src="./assets/dh8nH4lS_400x400.jpg">
        <h1>{{ profileData.name}}</h1>
        <h4 class="location">{{ profileData.location }}</h4>
        <h4>{{ profileData.about }}</h4>
        <div class="links">
            <Links />
        </div>
    </div>
</template>


<style scoped>
.container{
    display: flex;
    align-items: center;
    flex-direction: column;
    background: #333;
    width: 300px;
    max-width: 80%;
    border-radius: 30px;
    padding: 40px;
}
img{
    width: 170px;
    border-radius: 100%;
}
h1{
    font-size: 1.8rem;
    margin-bottom: 0;
}

.location{
    font-size: 1rem;
    color: rgb(0, 209, 0);
    margin: 10px 0 0 0;
}
h4{
    margin: 10px 0;
}

.links{
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;   
}
</style>