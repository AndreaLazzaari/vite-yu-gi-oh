<template lang="">

<AppHeader/>

<main>

</main>
</template>

<script>
import AppHeader from '../src/components/AppHeader.vue';

export default {
  data() {
    return {
      components: {
        AppHeader
      },
    }
  },
}
</script>
<style lang="scss">
  @use './styles/general.scss';

  main{
    background-color: #d48f38;
    height: 100vh;
  }
</style>
