<template>
  <div class="row">
    <q-item v-for="task in tasks" :key="task.id" class="column bg-grey">
      <q-item-lable>{{ task.title }}</q-item-lable>
      <q-item-lable>{{ task.description }}</q-item-lable>
      <q-btn no-caps outline color="white" text-color="white" label="Resume" />
    </q-item>
  </div>
</template>
<script>
export default {
  name: "DailyActivity",

  data() {
    return {
      tasks: [
        {
          id: 1,
          title: "Exercise",
          description: "You have 2 exercise",
        },
        {
          id: 2,
          title: "Online class",
          description: "You have 2 class",
        },
        {
          id: 3,
          title: "Conferance",
          description: "You have 2 confrance",
        },
      ],
    };
  },
};
</script>
<style></style>
