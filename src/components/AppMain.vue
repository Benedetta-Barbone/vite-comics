<script> 
import ListCards from './ListCards.vue';

export default {
    data() {
    },
    components:{
        ListCards,
    }
}

</script>

<template> 
<main>
   <ListCards />
</main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@use '../styles/general.scss' as *;


</style>