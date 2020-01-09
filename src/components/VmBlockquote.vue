<template>
  <blockquote>
  <p><em>{{ text }}</em></p>
</blockquote>
</template>

<script>
// je déclare la propos qui sera utilisé dans appvue
export default {
    name: 'VmBlockquote',
    props:['text']

}
</script>

<style>

</style>