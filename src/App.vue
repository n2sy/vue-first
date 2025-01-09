<script setup>
import First from './components/First.vue'
import Second from './components/Second.vue'
import GlobalStyle from './components/GlobalStyle.vue'
import LocalStyle from './components/LocalStyle.vue'
import ModularStyle from './components/ModularStyle.vue'
import MyEvent from './components/MyEvent.vue';
import MyReactiveComponent from './components/MyReactiveComponent.vue';
import ComputedProperties from './components/ComputedProperties.vue';
import ConditionalComponent from './components/ConditionalComponent.vue';
import IterativeComponent from './components/IterativeComponent.vue';
import TwoWayBindingComponent from './components/TwoWayBindingComponent.vue'
import StaticProps from './components/StaticProps.vue'
import DynamicProps from './components/DynamicProps.vue'
import ComponentEvent from './components/ComponentEvent.vue'
import SlotComponent from './components/SlotComponent.vue'

import { ref } from 'vue'
import FallbackComponent from './components/FallbackComponent.vue'
let prenom = ref("nidhal");
let nom = ref("jelassi")

function lireEvent(param1, param2) {
    console.log(param1, param2);
    
    prenom.value = param1;
}
</script>

<template>
 <!-- <First></First>
 <Second></Second> -->
 
 
 <!-- <GlobalStyle></GlobalStyle>
 <LocalStyle></LocalStyle>
 <ModularStyle></ModularStyle> -->
 
 <!-- 
 <MyEvent></MyEvent>-->
  
  <!-- <MyReactiveComponent></MyReactiveComponent> -->
   
   <!-- <ComputedProperties></ComputedProperties> -->
    
    <!-- <ConditionalComponent></ConditionalComponent> -->
    <!-- <IterativeComponent></IterativeComponent> -->
     
   <!-- <TwoWayBindingComponent></TwoWayBindingComponent> -->
    
    <!-- <StaticProps name="nidhal" age=20></StaticProps>  -->
     
     <!-- <DynamicProps :p1="prenom" :p2="nom" :p3="30"></DynamicProps> -->
     <!-- <DynamicProps :p1="prenom"  :p3="300"></DynamicProps> -->
      
    <!-- <h2>{{  prenom  }}</h2>
      <ComponentEvent @mary="console.log('hey mary')" @maryevent="lireEvent"></ComponentEvent> -->
      
      
     <!-- La syntaxe <SlotComponent /> ne marche pas -->
     <!-- <SlotComponent>
        <h1>My content slot</h1>
     </SlotComponent>  -->
     
     <FallbackComponent></FallbackComponent>
     <FallbackComponent><p>I pass this time a slot, so no fallback</p></FallbackComponent>
</template>

<style scoped>
</style>
