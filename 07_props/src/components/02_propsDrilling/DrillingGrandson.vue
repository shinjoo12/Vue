<script setup>
 import {inject , ref, updated} from 'vue';

 const propsCount = inject("count");

 updated(){
    console.log("grandson update")
 }
</script>

<template>
    <h3>grandson : {{ propsCount }}</h3>
    <button @click = "propsCount++">{{ propsCount }}</button>
</template>