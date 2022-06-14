<template>
  <hr />
  Form Handling
  <form @submit.prevent="handleSubmit">
    <input type="text" v-model="data.name" placeholder="Nama">
    <p>{{msg.name}}</p>
    <input type="number" v-model="data.age"  placeholder="Age">
    <p>{{msg.age}}</p>
   <button type="submit" >Submit Now</button>
  </form>
</template>
<script>
  export default {
    name:"FormHandling",
    data(){
      return {
        data:{
          name:"",
          age:""
        },
        msg:{
          name:"",
          age:""
        }
      }
    },
    methods:{
      handleSubmit(){
        if(this.data.name==""){
          this.msg.name="Name is required"
        }
        else if(this.data.age==""){
          this.msg.age="age is required"
        }
      }
    }
  }
</script>
<style scoped>
  form input{
    padding: 10px;
    display: block;
    margin: 5px auto;
  }
</style>