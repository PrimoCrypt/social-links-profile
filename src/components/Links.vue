<script setup>
import { profileData } from '../data.js';
</script>

<template>
    <div class="link" v-for="link in profileData.links">
        <button>{{ link.linkName }}</button>
    </div>
</template>

<style>
.link{
    max-width: 100%;
    margin-bottom: 20px;
}
.link:last-child{
    margin-bottom: 0;
}
button:hover{
    border: 1px rgb(0, 209, 0) solid;
}
button:active{
    background: rgb(0, 209, 0);
}
</style>