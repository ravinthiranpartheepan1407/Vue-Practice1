<template>
  <v-container>
    <v-layout>
      <template v-for="(data, next) in datas">
        <v-card :key="next">
          <p>{{data.firstname}}</p>
          <p>{{data.lastname}}</p>
        </v-card>
        
        <v-card :key="next">
          <p>{{data.course}}</p>
          <p>{{data.Year}}</p>
        </v-card>
      </template>
    </v-layout>
  </v-container>
</template>

<script>
  export default{
    name: 'Resume',
    data: ()=>({
      datas: [
        {
          firstname: 'Ravinthiran',
          lastname: 'Partheepan'
        },
        {
          course: 'Master of Applied Informatics',
          Year: '2019-2021'
        },
      ],
    })
  }
</script>
