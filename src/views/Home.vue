<template>
  <span>
    <HomeContent />
    <Items />

  </span>
</template>

<script>
import Items from '../components/Items';
import HomeContent from '../components/HomeContent';
export default {
    name: 'Home',

    components: {
        Items,
        HomeContent
    },
};
</script>
