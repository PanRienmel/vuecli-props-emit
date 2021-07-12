<template>
  <div>
      <input type="text" placeholder="Search..."
      v-model="inputText"
      @keyup.enter="$emit('ricerca', inputText)">
  </div>
</template>

<script>
export default {
    name:"Search",
    data(){
        return{
            inputText: ""
        }
    }
}
</script>

<style>

</style>