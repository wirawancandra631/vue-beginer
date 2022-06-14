<template>
  <hr />
  Transisi 
  <button @click="status=true">Star</button>
  <button @click="status=false">Finish</button>
  
  <Transition>
      <p v-if="status">Lorem ipsum dolor sit amet.</p>
  </Transition>

</template>
<script>
  export default {
    name:"TransitionFeature",
    data(){
      return {
        status:false
      }
    }
  }
</script>