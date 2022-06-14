<template>
  <hr />
  <button @click="focus">Aktiv</button>
  <input type="text" ref="focus"/>
</template>
<script>
  export default {
    name:"RefsFeature",
    methods:{
      focus(){
        this.$refs.focus.focus();
        console.log(this.$refs)
      }
    }
  }
</script>