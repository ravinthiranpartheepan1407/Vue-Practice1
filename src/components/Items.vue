<template>
  <span>
  <v-container>

      <template v-for="(prod, next) in product">
        <v-card :key="next">
          <p style="text-align: center">{{prod.title}}</p>
          <p style="text-align: center">{{prod.link}}</p>
        </v-card>
      </template>

  </v-container>
  </span>
</template>

<script>
  export default {
    name: 'Items',
    data (){
      return{
          product: [
            {
              title: 'Platinum',
              link: 'https://ravinthiranpartheepan.com',
            },
            {
              title: 'Gold',
              link: 'https://ravinthiranpartheepan.com/shop',
            },
            {
            title: 'Silver',
            link: 'https://ravinthiranpartheepan.com/ethapp',
            },

          ],
      };
    }
  };
</script>
