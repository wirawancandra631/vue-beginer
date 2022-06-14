<template>
  <hr />
  <p>List Rendering</p>
  <table>
    <thead>
      <tr>
        <th>No</th>
        <th>Nama</th>
        <th>Age</th>
      </tr>
    </thead>
    <tbody>
     <template v-for="(value,index) in data" :key="index">
       <tr>
         <td>{{index+1}}</td>
         <td>{{value.name}}</td>
         <td>{{value.age}}</td>
       </tr>
     </template>
    </tbody>
  </table>
</template>
<script>
  export default {
    name:"ListRendering",
    data(){
      return {
        data:[
          {name:"Jhon",age:10},
          {name:"Foo",age:12},
          {name:"Mark",age:14},
          {name:"Zero",age:18},
          {name:"Brucee",age:20},
          
          ]
      }
    }
  }
</script>
<style scoped="">
  table{
    width: 80%;
    margin: auto;
  }
  table tr td{
    padding: 5px;
  }
</style>