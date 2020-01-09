<template>
  <div id="app">
   appel du component avec une props
    <!-- 3 - j'utilise -->
  <VmBlockquote text="Mon texte"></VmBlockquote>
  équivalent à
<blockquote>
  <p><em>Yeah!! Milligram is amazing.</em></p>
</blockquote>

Les boutons :
<a class="button" href="#">Default Button</a>

<button class="button button-outline">Outlined Button</button>

<input class="button button-clear" type="submit" value="Clear Button">

  </div>
</template>

<script>
// 1 - j'importe
import VmBlockquote from './components/VmBlockquote'
// 2  je déclare
export default {
  name: 'app',
  // j'injecte le VMBlockquote après l'avoir importé
  components: {VmBlockquote}  
}
</script>

<style>
</style>
