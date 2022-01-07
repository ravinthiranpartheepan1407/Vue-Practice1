<template>
  <v-container>

      <template v-for="(data, next) in datas">
        <v-card :key="next">
        <p style="text-align: center">{{data.firstname}}</p>
          <p style="text-align: center">{{data.lastname}}</p>
        </v-card>

        <v-card :key="next">
          <p style="text-align: center">{{data.course}}</p>
          <p style="text-align: center">{{data.Year}}</p>
        </v-card>
      </template>

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
