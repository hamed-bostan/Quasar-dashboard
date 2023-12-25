<template>

 <div class="Package-inventory-main-container example-row-all-breakpoints row" >
   <div
   v-for="item in items" :key="item.id">
        <div class="col-2">
            <q-item-lable>
              {{item.text}}
            </q-item-lable>
            <div class="packageInventory-desc">
              <q-img
              src='../assets/images/Ellipse.png'
              spinner-color="white"
              style="height: 2.5rem; max-width: 2.5rem"
            />
            <q-item-lable>{{item.description}}</q-item-lable>
            </div>
        </div>
      </div>
 </div>

</template>
<script setup lang="ts">
import { ref } from "vue";

const items = ref([
  {
  id:1,
  text:"Day",
  description:"inventory1"
},
{
  id:2,
  text:"Conferance",
  description:"inventory2"
},
{
  id:3,
  text:"Exercise",
  description:"inventory3"
},
{
  id:4,
  text:"Online class",
  description:"inventory4"
},
]);
</script>
<style >
.Package-inventory-main-container{
  gap: 1.5rem;
}

.col-2{
  display: flex;
  flex-direction: column;
  row-gap: 1.5rem;
  padding: 0.5rem;
  background: #A5A5A5;
  width: 10.5rem;
  height: 7.25rem;
}

.packageInventory-desc{
  display: flex;
  column-gap: .75rem;
  align-items: center;
}

</style>
