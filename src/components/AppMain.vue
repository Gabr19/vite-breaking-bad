<script>
import SearchForm from './SearchForm.vue';

export default {
  name: 'AppMain',
  props: {
    charactersList: {
      type: Array,
      default: []
    }
  },
  components:{
    SearchForm,
  }
}
</script>

<template>

  <div class="container_grande">
    <div class="container container_medio">
      <div class="my_search"
>
        <SearchForm/>

      </div>
      <div class="container container_piccolo p-5">
        <div class="found_bar">
          Found 39 cards
        </div>
        <div class="container_card d-flex flex-wrap justify-content-between ">
          <div class="my_card" v-for="character in charactersList">
            <div class="my_img">
              <img id="img_card" :src="character.card_images[0].image_url" alt="">
            </div>
            <div id="my_text">
              {{character.name}}
              {{ character.archetype }}
            </div>
          </div>
          
        </div>
        

      </div>

    </div>

  </div>

  


</template>

<style lang="scss" scoped>

</style>
