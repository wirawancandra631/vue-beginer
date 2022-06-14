<template>
  <hr />
  <button @click="showText">Show Text</button>
  <p v-show="show">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta, ducimus.</p>
  <hr />
  <small>Check Number if number > 0 text change to great else text change small</small>
  <p>Check number is {{number}} message is {{msg}} </p>
  <button @click="number++">Increment</button>
  <button @click="number--">Decrement</button>
</template>
<script>
  export default {
    name:"ConditionalRendering",
    data(){
      return {
        show:false,
        number:0,
        msg:"Netral"
      }
    },
    methods:{
      showText(){
        (this.show) ? this.show=false :this.show=true
      }
    },
    watch:{
      number(newvalue){
        (newvalue>0)?this.msg="great" :this.msg="small"
      }
    }
  }
</script>