<template>
  <hr />
  <button @click="isActive='TabA'">Tab A</button>
  <button @click="isActive='TabB'">Tab B</button>
<keep-alive>
  <component :is="isActive"></component>
</keep-alive>

</template>
<script>
import TabA from './TabA.vue';
import TabB from './TabB.vue';
  export default {
    name:"DynamicComponent",
    data(){
      return {
        isActive:"TabA"
      }
    },
    components:{
      TabA,
      TabB
    }
  }
</script>