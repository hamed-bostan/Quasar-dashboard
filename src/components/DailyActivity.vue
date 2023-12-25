<template>
  <div class="daily-activity-main-container row">
    <q-item v-for="task in tasks" :key="task.id" class="daily-activity column">
    <q-img
      :src='task.image'
      spinner-color="white"
      style="height: 5rem; max-width: 5rem"
    />
    <div class="daily-activity-text">
      <q-item-lable>{{ task.title }}</q-item-lable>
      <q-item-lable>{{ task.description }}</q-item-lable>
    </div>
      <q-btn no-caps outline color="white" text-color="white" label="Resume" class="daily-activity-btn"/>
    </q-item>
  </div>
</template>
<script setup lang="ts">
import { ref } from "vue";

const tasks = ref([
  {
    id: 1,
    title: "Exercise",
    description: "You have 2 exercise",
    image: 'https://picsum.photos/500/300'
  },
  {
    id: 2,
    title: "Online class",
    description: "You have 2 class",
     image: 'https://picsum.photos/500/300'
  },
  {
    id: 3,
    title: "Conferance",
    description: "You have 2 confrance",
     image: 'https://picsum.photos/500/300'
  },
]);

const urlMaker = (url:string)=>{
  return new URL(url)
}
</script>
<style>

.daily-activity-main-container{
  display: flex;
  column-gap: 1rem;
  background: green;
}

.daily-activity{
  width: 14.8125rem;
  height: 16rem;
  justify-content: center;
  align-items: center;
  background: #A5A5A5;
  display: flex;
  row-gap: 1.5rem;
}

.daily-activity-text{
  display: flex;
  text-align: center;
  flex-direction: column;
}

.daily-activity-btn{
  width: 12.5rem;
  height: 2rem;
}
</style>
