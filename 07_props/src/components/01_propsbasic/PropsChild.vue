<script setup>
import {inject} from 'vue';

// inject 주입하다
//inject("전달한 key값");
const message = inject('data');  //객체 형식의 데이터
const darkMode = inject("darkMode");
const darkState = inject("darkState");

// const message1 = inject("message"); //단일 데이터
// console.log(message)

</script>

<template>
    

    <h3>전달 받은 props : {{message}}</h3>

    <button @click ="darkMode">자식의 DarkMode + {{darkState}} </button>
</template>