<script>
export default {
    name: 'SingleCard',
    
    props: {
        comic: {
            type: Object,
            required: true
    }
}

}
</script>


<template> 
   <div class="card">
    <img :src="comic.thumb" alt="Comic thumbnail" class="card-img">
    <div class="card-details">
      <h2>{{ comic.series }}</h2>

    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@use '../styles/general.scss' as *;

.card { 
  margin: 10px;
  width: 200px;
}

.card-img {
  width: 100%;
  height: 270px;
}

h2 {
  font-size: 1.2em;
  margin: 10px 0;
}

</style>