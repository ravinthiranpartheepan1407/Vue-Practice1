<template>
    <v-app>
    <AppNavigation></AppNavigation>
        <v-content transition="slide-x-transition">
          <router-view>

          </router-view>
        </v-content>
      <Footer />
    </v-app>
</template>

<script>
import AppNavigation from '@/components/AppNavigation';
import Footer from '@/components/Footer';
export default {
    name: 'App',
    components:{
      AppNavigation,
      Footer
    },
    data: () => ({
        //
    }),
};
</script>
