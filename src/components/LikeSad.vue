<script setup>
import { ref } from "vue";
const like = ref(0);
const sad = ref(0);

function likeClick(){
  like.value+=1;
}
function SadClick(){
  sad.value+=1;
}

</script>

<template>
    <div>
    <a href="#" class="btn btn-primary " @click="likeClick()"><i class="bi bi-hand-thumbs-up"></i></a>{{like}}
    <a href="#" class="btn btn-primary " @click="SadClick()"><i class="bi bi-emoji-frown-fill"></i></a>{{sad}}
    </div>
  </template>
  <style scoped> </style>