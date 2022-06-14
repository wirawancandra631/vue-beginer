<template>
  <hr />
  <p v-text="text"></p>
  <div v-html="html"></div>
  <p :class="bindclass">Bind Class</p>
</template>
<script>
  export default {
    name:"BindFeature",
    data(){
      return {
        text:"Bind Text",
        html:"<b>Bind Html</b>",
        bindclass:"bindclass"
      }
    }
  }
</script>
<style>
  .bindclass{
    color: blue;
  }
</style>