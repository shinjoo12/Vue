<script setup>
import {inject, ref, onUpdated} from 'vue';
import Grandson from "./DrillingGrandson.vue"

const propsCount = inject("count");

onUpdated(){
    console.log("child~~ update");
}

</script>

<template>
    <h2>child : {{propsCount }}</h2>
    <Grandson/>
</template>