<template>
<div>
 <!--
    <h1 v-if="type==='1'">{{texte}}</h1>
  <h2 v-else-if="type==='2'">{{texte}}</h2>
  <h3 v-else-if="type==='3'">{{texte}}</h3>
  <h4 v-else-if="type==='4'">{{texte}}</h4>
  <h5 v-else-if="type==='5'">{{texte}}</h5>
  <h6 v-else-if="type==='6'">{{texte}}</h6>
  -->
  <component :is="elementAAfficher">{{texte}}</component>
  </div>
</template>

<script>

export default {
    name: 'VmHeading',
    props: [ 'type', 'texte'],
    computed: {
      elementAAfficher () {
        return `h${this.type}`
        //peut aussi s'écrire
        //return "h" + this.type
      }
    }
  
}


</script>

<style>

</style>