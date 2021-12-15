<template>
  <img id="Image_Tringle" src="./assets/tringles-rail.jpeg">
  <HelloWorld msg="Acheter une tringle à rideau personnalisée"/>

  <!-- Première étape -->
  <div class="Premièreétape" v-if="étape === 'Premièreétape'">
  <h1>Etape 1</h1>
  <Number_input msg=" "/> 
  <button id="button_Premièreétape" v-on : click="étape=Deuxièmeétape"> Suite </button>
  </div>


  <!-- Deuxième étape -->
  <div class="Deuxièmeétape" v-if="étape === 'Deuxièmeétape'">
  <h1>Etape 2</h1>
  <Number_input msg=" "/> 
  <button id="button_Pemièreétape" v-on : click="étape=Troisièmeétape"> Suite </button>
  </div>



  <!-- Troisième étape -->
  <div class="Troisièmeétape" v-if="étape === 'Troisièmeétape'">
  <h1>Etape 3</h1>
  <Number_input msg=" "/> 
  <button id="button_Premièreétape" v-on : click="étape=Premièreétape"> Ajouter au panier </button>
  </div>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Ajouter_au_panier from './components/Ajouter_au_panier.vue'
import Couleur from './components/Couleur.vue'
import RadioBoutton from './components/RadioBoutton.vue'
import Numberinput from '.components/Numberinput.vue'
export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
