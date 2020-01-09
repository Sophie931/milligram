<template>
  <div id="app">
   appel du component avec une props
    <!-- 3 - j'utilise -->
  <VmBlockquote text="Mon texte"></VmBlockquote>
  équivalent à
<blockquote>
  <p><em>Yeah!! Milligram is amazing.</em></p>
</blockquote>

Les titres :
<VmHeading type="1" texte="Mon titre 1"></VmHeading> equivalent <h1>Mon titre 1</h1>
<VmHeading type="2" texte="Mon titre 2"></VmHeading> equivalent <h2>Mon titre 2</h2>
<VmHeading type="3" texte="Mon titre 3"></VmHeading> equivalent <h3>Mon titre 3</h3>
<VmHeading type="4" texte="Mon titre 4"></VmHeading> equivalent <h4>Mon titre 4</h4>
<VmHeading type="5" texte="Mon titre 5"></VmHeading> equivalent <h5>Mon titre 5</h5>
<VmHeading type="6" texte="Mon titre 6"></VmHeading> equivalent <h6>Mon titre 6</h6>

  </div>
</template>

<script>
// 1 - j'importe
import VmBlockquote from './components/VmBlockquote'
import VmHeading from './components/VmHeading'
// 2  je déclare
export default {
  name: 'app',
  // j'injecte le VMBlockquote après l'avoir importé
  components: {
    VmBlockquote,
    VmHeading
  },  
}
</script>

<style>
</style>
