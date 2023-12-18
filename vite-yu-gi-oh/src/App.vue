
<script>
import { store } from './js/store.js';
import axios from 'axios';
import AppHeader from './components/AppHeader.vue';
import AppCardList from './components/AppCardList.vue';

export default {
  components: {
        AppHeader,
        AppCardList,
      },

  data() {
    return {
      store,
    }
  },
  methods: {
    getCard() {
        axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0')
      .then((response) => {
        // handle success
        console.log(response);
        this.store.cardList = data.data;
      })
      .catch(function (error) {
        // handle error
        console.error(error);
      })
    }
  },
  created() {
    this.getCard();
  },
}
</script>


<template lang="">

<AppHeader/>
<main>

<AppCardList/>

</main>
</template>

<style lang="scss">
  @use './styles/general.scss';

  main{
    background-color: #d48f38;
    width: 100%;
    height: 100vh;
    padding: 1.5rem;
  }
</style>
