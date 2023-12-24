<template lang="">
  <div class="q-pa-md">
    <q-markup-table square separator>
      <thead>
        <tr>
          <th class="text-left">physiotherapist</th>
          <th class="text-right">date</th>
          <th class="text-right">type</th>
          <th class="text-right">xx</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="text-left">Hosein jalalian</td>
          <td class="text-right">1/1/2022</td>
          <td class="text-right">online</td>
          <td class="text-right">
            <q-btn outline style="color: goldenrod;" label="more" />
          </td>
        </tr>

        <tr>
          <td class="text-left">Hosein jamalian</td>
          <td class="text-right">1/1/2022</td>
          <td class="text-right">offline</td>
          <td class="text-right">more</td>
        </tr>

        <tr>
          <td class="text-left">Alireza Ahmadi</td>
          <td class="text-right">1/1/2022</td>
          <td class="text-right">offline</td>
          <td class="text-right">more</td>
        </tr>

        <tr>
          <td class="text-left">Mahsa Amini</td>
          <td class="text-right">1/1/2022</td>
          <td class="text-right">online</td>
          <td class="text-right">more</td>
        </tr>
      </tbody>
    </q-markup-table>
  </div>
</template>
<script>
export default {
  name: "EvaluationPhysiotherapist",
};
</script>
<style lang=""></style>
