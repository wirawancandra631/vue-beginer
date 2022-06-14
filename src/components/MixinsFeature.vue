<template>
  <hr />
  <p>Mixins Feature</p>
  <p>Num {{num}}</p>
</template>
<script>
 import mixins from './mixins';
  export default {
    name:"MixinsFeature",
    mixins:[mixins]
  }
</script>