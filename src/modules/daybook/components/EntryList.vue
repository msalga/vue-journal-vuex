<template>
  <div class="entry-list-container">
    <div class="px-2 pt-2">
      <input type="text" class="form-control" placeholder="Buscar entrada" />
    </div>

    <div class="entry-scrollarea">
      <Entry v-for="item in 10" :key="item"/>
    </div>
  </div>
</template>

<script>
import { defineAsyncComponent } from 'vue';

export default {
  components:{
    Entry:  defineAsyncComponent(()=> import ('./Entry.vue'))
  }
};
</script>

<style lang="scss" scoped>
.entry-list-container
{
  border-right: 1px solid #2c2e9e;
  height: calc( 100hv - 56px)
  
}
  
  .entry-scrollarea
{
  height: calc( 100hv - 110px);
  overflow:scroll
}
</style>