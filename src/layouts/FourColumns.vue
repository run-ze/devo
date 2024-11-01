<template>
  <div id="four-columns-wrapper">
    <platform-card :cardIndex="0"></platform-card>
    <platform-card :cardIndex="1"></platform-card>
    <platform-card :cardIndex="2"></platform-card>
    <platform-card :cardIndex="3"></platform-card>
  </div>
</template>

<script>
import PlatformCard from '../components/PlatformCard.vue';

export default {
  name: 'FourColumns',
  components: {
    PlatformCard,
  },
};
</script>

<style scoped>
#four-columns-wrapper {
  display: grid;
  grid-gap: 0.5rem;
}

@media screen and (min-width: 1200px) {
  #four-columns-wrapper {
    grid-template-columns: repeat(4, 1fr);
    height: 100%;
  }
}
</style>
