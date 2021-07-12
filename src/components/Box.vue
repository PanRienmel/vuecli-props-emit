<template>
  <div>{{title}}
    <img :src="img" :alt="oggetto.desc">
  </div>
</template>

<script>
export default {
    name: 'Box',
    props: {
      img: String,
      title: String,
      oggetto: Object
    }
}
</script>

<style>

</style>