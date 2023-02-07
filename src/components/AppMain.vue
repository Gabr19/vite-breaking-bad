<script>
import SearchForm from './SearchForm.vue';

export default {
  name: 'AppMain',
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
          <div class="my_card" v-for="i in 20">
            <div class="my_img">
              <img id="img_card" src="https://upload.wikimedia.org/wikipedia/commons/3/3c/IMG_logo_%282017%29.svg" alt="">
            </div>
            <div id="my_text">
              prova
            </div>
          </div>
          
        </div>
        

      </div>

    </div>

  </div>

  


</template>

<style lang="scss" scoped>

</style>
