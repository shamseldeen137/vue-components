<template>
  <!-- <Card >
Card Content
  </Card>
  <Card>
<h2> Card Content</h2>
  </Card>


<Card>
<template v-slot:card-header>
  <h3> This is Card Header</h3>
</template>
<template v-slot:default>
  <img src="https://picsum.photos/200"/>
</template>
<template v-slot:card-footer>
  <h4> This is Card Footer</h4>
  <button> View Details</button>
</template>
</Card> -->

<!-- <NameList >
  <template v-slot:default="slotProps">
    <span style="color: red"> {{ slotProps.fristName }}</span>

  </template>
</NameList>
<NameList >
  <template v-slot:default="slotProps">
    <span style="color: red"> {{ slotProps.fristName }} {{ slotProps.lastName }}</span>

  </template>
</NameList> -->


<!-- <h4>
  This is App Component
</h4>
<ChildStyle >
  

  <h4>
    This is Child Style Component
</h4>
  
  
  </ChildStyle> -->
<button @click="activTab='TabA'"> Tab A</button>
<button @click="activTab='TabB'"> Tab B</button>
<button @click="activTab='TabC'"> Tab C</button>
<!-- 
<TabA  v-if="activTab==='TabA'"/>
<TabB  v-if="activTab==='TabB'"  />
<TabC  v-if="activTab==='TabC'"/> -->
<component :is="activTab"/>


</template>

<script>
//import Card from './components/Card.vue';
//import NameList from './components/NameList.vue';
//import ChildStyle from './components/ChildStyle.vue';
import TabA from './components/TabA.vue';
import TabB from './components/TabB.vue';
import TabC from './components/TabC.vue';
export default {
  name: 'App',
  components: {
    // Greet,
    //ComponentC,
    //Card,
   // NameList
    //ChildStyle,
    TabA,
    TabB,
    TabC

    
  },
  data() {
    return {
    activTab:'TabA'
      
    }
  },
  
}
</script>

<style >
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;

}
h4 {
  color: orange;
}
</style>
