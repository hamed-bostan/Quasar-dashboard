<template lang="">
  <div>
    <div class="chat-names row">
      <q-item v-for="name in names" :key="name.id">{{ name.name }}</q-item>
    </div>
  </div>
</template>
<script>
export default {
  name: "Chat",
  data() {
    return {
      names: [
        {
          id: 1,
          name: "Hosein",
        },
        {
          id: 2,
          name: "Hosein J",
        },
        {
          id: 3,
          name: "Alireza",
        },
        {
          id: 4,
          name: "Alireza J",
        },
      ],
    };
  },
};
</script>
<style >
.chat-names{
  background: pink;
}
</style>
