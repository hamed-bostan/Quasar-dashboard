<template>
  <div class="main-container">
    <div class="row">
      <div class="col-8">
        <DailyActivity />
      </div>
        <div class="col-4">
          <PackageInventory />
        </div>
    </div>

    <div class="row">
      <div class="col-8">
        <EvaluationPhysiotherapist />
      </div>
      <div class="col-4">
        <Chat />
      </div>
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
  /* width: 90rem; */
  width: 100%;
  height: 100vh;
  /* display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center; */
}
</style>
