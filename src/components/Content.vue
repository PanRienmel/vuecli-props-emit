<template>
  <div>
    {{msg}}
    <Box v-for="(obj, index) in objects" :key="index" :img="obj.img" :title="obj.text" :oggetto="obj"/>
  </div>
</template>

<script>
import Box from '@/components/Box.vue'
export default {
  name: 'Content',
  components: {
    Box
  },
  props: {
    msg: String
  },
  data(){
    return{
      objects: [
        {
          text: "Primo blocco",
          img: "https://picsum.photos/200/300?random=1",
          url: "#",
          desc: "Lorem ipsum"
        },
        {
          text: "Secondo blocco",
          img: "https://picsum.photos/200/300?random=2",
          url: "#",
          desc: "Lorem ipsum"
        },
        {
          text: "Terzo blocco",
          img: "https://picsum.photos/200/300?random=3",
          url: "#",
          desc: "Lorem ipsum"
        }
      ]
    }
  }
}
</script>

<style>

</style>