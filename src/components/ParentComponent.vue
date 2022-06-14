<template>
  <hr />
  <p>Parent Component</p>
  <template v-for="n in 5" :key="n">
    <SlotFeature>{{n}}</SlotFeature>
  </template>
</template>
<script>
  import SlotFeature from './SlotFeature.vue'
  export default {
    name:"ParentComponent",
    components:{
      SlotFeature
    }
  }
</script>