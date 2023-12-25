<template>
  <div >
    <q-table
      class="table-class"
      flat
      hide-bottom
      square
      :rows="rows"
      :columns="columns"
      row-key="name"
    />
  </div>
</template>

<script>
const columns = [
  { label: 'Physiotherapist', field: row => row.name, align: 'left', },
  { label: 'Date', field: 'date',align: 'left',},
  { label: 'Type', field: 'type' , align: 'left'},
  { field: 'more' , align: 'right'},
]

const rows = [
  {
    name: 'Hosein jalalian',
    date: "1/1/2022"  ,
    type: "online" ,
    more: "more",
  },
  {
    name: 'Hosein jamalian',
    date: "1/1/2022",
    type: "offline",
    more: "more",
  },
  {
    name: 'Alireza Ahmadi',
    date:" 1/1/2022",
    type: "offline",
    more: "more",
  },
  {
    name: 'Mahsa Amini',
    date: "1/1/2022",
    type: "online",
    more: "more",
  },
]

export default {
  setup () {
    return {
      columns,
      rows
    }
  }
}
</script>

<style >

.table-class {
  background: #A5A5A5;
}

</style>
