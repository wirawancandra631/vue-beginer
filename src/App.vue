<template>
  <h6>Vue</h6>
  <TemplateFeature/>
  <BindFeature/>
  <ConditionalRendering/>
  <ListRendering/>
  <FormHandling/>
  <ParentComponent/>
  <DynamicComponent/>
  <RefsFeature/>
  <TransitionFeature/>
  <MixinsFeature/>
</template>
<script>
  import TemplateFeature from './components/TemplateFeature.vue'
  import BindFeature from './components/BindFeature.vue';
  import ConditionalRendering from './components/ConditionalRendering.vue'
  import ListRendering from './components/ListRendering.vue'
  import FormHandling from './components/FormHandling.vue'
  import ParentComponent from './components/ParentComponent.vue'
  import DynamicComponent from './components/DynamicComponent.vue'
  import RefsFeature from './components/RefsFeature.vue'
  import TransitionFeature from './components/TransitionFeature.vue'
  import MixinsFeature from './components/MixinsFeature.vue'
  export default {
    name:"App",
    components:{
      TemplateFeature,
      BindFeature,
      ConditionalRendering,
      ListRendering,
      FormHandling,
      ParentComponent,
      DynamicComponent,
      RefsFeature,
      TransitionFeature,
      MixinsFeature
    }
  }
</script>
<style>
  body{
    color: black;
    text-align: center;
  }
</style>