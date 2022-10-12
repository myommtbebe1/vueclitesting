<template>

  <h1>Hello</h1>
  <div v-if="showModal"> 
    <Modal :header="header" content="welcome user" @close="showModal=false" />
  </div>
 
  <button @click="showModal=true">open modal</button>
</template>

<script>
import Modal from "./components/Modal-m.vue"
export default {
  data(){
    return{
      header:'Facebook',
      title:"you donno js",
      showModal:false,
    }
  },
  method:{
    
  },
  components:{
    Modal
  }
}
</script>

<style scoped>
 h1{
  color:blue;
 }
</style>