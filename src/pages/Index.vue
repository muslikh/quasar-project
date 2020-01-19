<template>
  <q-page>
    <div>
       <q-select
      v-model="select"
      :options="selectOptions"
    />
    <br>
    <div class="q-pa-md">
      <q-table
      title="Jadwal Sholat Di Pasuruan "
      :data="data"
      :columns="columns"
      row-key="name"
      />
    </div>
    <div id="app">
  {{ info }}
</div>
    </center>
    </div>
  </q-page>
</template>

<script>
export default {
  data () {
    return{
      selectOptions: [
        {
          label: 'Pasuruan',
          value: 'pas'
        },
        {
          label: 'Malang',
          value: 'mal'
        }
      ],
      columns:[
        {
        name: 'tgl',
        required:true,
        label : 'Tanggal',
        align: 'left',
        field: row => row.tgl,
        format: val => `${val}`,
        sortable:true
        },
        {
        name: 'Subuh',
        required:true,
        label : 'Subuh',
        align: 'left',
        field: row => row.Subuh,
        format: val => `${val}`,
        sortable:true
        },
        {
        name: 'Dhuhur',
        required:true,
        label : 'Dhuhur',
        align: 'left',
        field: row => row.Dhuhur,
        format: val => `${val}`,
        sortable:true
        },
        {
        name: 'Ashar',
        required:true,
        label : 'Ashar',
        align: 'left',
        field: row => row.Ashar,
        format: val => `${val}`,
        sortable:true
        },
        {
        name: 'Magrib',
        required:true,
        label : 'Magrib',
        align: 'left',
        field: row => row.Magrib,
        format: val => `${val}`,
        sortable:true
        },
        {
        name: 'Isya',
        required:true,
        label : 'Isya',
        align: 'left',
        field: row => row.Isya,
        format: val => `${val}`,
        sortable:true
        },
      ],data:[{tgl:'Rab 1 Jan',Subuh:'03:52',Dhuhur:'11:36',Ashar:'15:02',Magrib:'17:52',Isya:'19:08',},
{tgl:'Kam 2 Jan',Subuh:'03:53',Dhuhur:'11:36',Ashar:'15:02',Magrib:'17:52',Isya:'19:08',},
{tgl:'Jum 3 Jan',Subuh:'03:53',Dhuhur:'11:36',Ashar:'15:02',Magrib:'17:53',Isya:'19:09',},
{tgl:'Sab 4 Jan',Subuh:'03:54',Dhuhur:'11:37',Ashar:'15:03',Magrib:'17:53',Isya:'19:09',},
{tgl:'Min 5 Jan',Subuh:'03:54',Dhuhur:'11:37',Ashar:'15:03',Magrib:'17:54',Isya:'19:09',},
{tgl:'Sen 6 Jan',Subuh:'03:55',Dhuhur:'11:38',Ashar:'15:03',Magrib:'17:54',Isya:'19:09',},
{tgl:'Sel 7 Jan',Subuh:'03:56',Dhuhur:'11:38',Ashar:'15:04',Magrib:'17:54',Isya:'19:10',},
{tgl:'Rab 8 Jan',Subuh:'03:56',Dhuhur:'11:39',Ashar:'15:04',Magrib:'17:55',Isya:'19:10',},
{tgl:'Kam 9 Jan',Subuh:'03:57',Dhuhur:'11:39',Ashar:'15:04',Magrib:'17:55',Isya:'19:10',},
{tgl:'Jum 10 Jan',Subuh:'03:57',Dhuhur:'11:40',Ashar:'15:04',Magrib:'17:55',Isya:'19:11',},
{tgl:'Sab 11 Jan',Subuh:'03:58',Dhuhur:'11:40',Ashar:'15:05',Magrib:'17:56',Isya:'19:11',},
{tgl:'Min 12 Jan',Subuh:'03:59',Dhuhur:'11:40',Ashar:'15:05',Magrib:'17:56',Isya:'19:11',},
{tgl:'Sen 13 Jan',Subuh:'03:59',Dhuhur:'11:41',Ashar:'15:05',Magrib:'17:56',Isya:'19:11',},
{tgl:'Sel 14 Jan',Subuh:'04:00',Dhuhur:'11:41',Ashar:'15:05',Magrib:'17:57',Isya:'19:11',},
{tgl:'Rab 15 Jan',Subuh:'04:00',Dhuhur:'11:41',Ashar:'15:05',Magrib:'17:57',Isya:'19:11',},
{tgl:'Kam 16 Jan',Subuh:'04:01',Dhuhur:'11:42',Ashar:'15:05',Magrib:'17:57',Isya:'19:12',},
{tgl:'Jum 17 Jan',Subuh:'04:02',Dhuhur:'11:42',Ashar:'15:06',Magrib:'17:57',Isya:'19:12',},
{tgl:'Sab 18 Jan',Subuh:'04:02',Dhuhur:'11:43',Ashar:'15:06',Magrib:'17:57',Isya:'19:12',},
{tgl:'Min 19 Jan',Subuh:'04:03',Dhuhur:'11:43',Ashar:'15:06',Magrib:'17:58',Isya:'19:12',},
{tgl:'Sen 20 Jan',Subuh:'04:03',Dhuhur:'11:43',Ashar:'15:06',Magrib:'17:58',Isya:'19:12',},
{tgl:'Sel 21 Jan',Subuh:'04:04',Dhuhur:'11:43',Ashar:'15:06',Magrib:'17:58',Isya:'19:12',},
{tgl:'Rab 22 Jan',Subuh:'04:05',Dhuhur:'11:44',Ashar:'15:06',Magrib:'17:58',Isya:'19:12',},
{tgl:'Kam 23 Jan',Subuh:'04:05',Dhuhur:'11:44',Ashar:'15:06',Magrib:'17:58',Isya:'19:12',},
{tgl:'Jum 24 Jan',Subuh:'04:06',Dhuhur:'11:44',Ashar:'15:06',Magrib:'17:58',Isya:'19:12',},
{tgl:'Sab 25 Jan',Subuh:'04:06',Dhuhur:'11:44',Ashar:'15:06',Magrib:'17:58',Isya:'19:12',},
{tgl:'Min 26 Jan',Subuh:'04:07',Dhuhur:'11:45',Ashar:'15:05',Magrib:'17:58',Isya:'19:12',},
{tgl:'Sen 27 Jan',Subuh:'04:07',Dhuhur:'11:45',Ashar:'15:05',Magrib:'17:59',Isya:'19:12',},
{tgl:'Sel 28 Jan',Subuh:'04:08',Dhuhur:'11:45',Ashar:'15:05',Magrib:'17:59',Isya:'19:12',},
{tgl:'Rab 29 Jan',Subuh:'04:08',Dhuhur:'11:45',Ashar:'15:05',Magrib:'17:59',Isya:'19:12',},
{tgl:'Kam 30 Jan',Subuh:'04:09',Dhuhur:'11:46',Ashar:'15:05',Magrib:'17:59',Isya:'19:11',},
{tgl:'Jum 31 Jan',Subuh:'04:09',Dhuhur:'11:46',Ashar:'15:05',Magrib:'17:59',Isya:'19:11',},,],
      getData() {
    const url = `http://smknprigen.sch.id/siakad/api/`;
    return axios.get(url).then(response => response.data);
}
  }
}}
</script>
