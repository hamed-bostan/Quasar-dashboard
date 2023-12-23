<template>
  <div class="main-container">
    <div class="row">
      <DailyActivity />
      <PackageInventory />
    </div>
    <div class="row">
      <EvaluationPhysiotherapist />
      <Chat />
    </div>
  </div>
</template>
<script>
import { defineComponent } from "vue";
import DailyActivity from "./components/DailyActivity.vue";
import PackageInventory from "./components/PackageInventory.vue";
import EvaluationPhysiotherapist from "./components/EvaluationPhysiotherapist.vue";
import Chat from "./components/Chat.vue";

export default defineComponent({
  name: "App",
  components: {
    DailyActivity,
    PackageInventory,
    EvaluationPhysiotherapist,
    Chat,
  },
});
</script>
<style>
.main-container {
  background: #525252;
  width: 90rem;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
