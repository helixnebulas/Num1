<template>
    <div> 
        <ul class= "list-group p-4 align-items-center" >
           <Items
              v-for="t of titles"
              v-bind:t="t"
           />
        </ul>
        
    </div>
</template>

<script>
import Items from '@/components/Items'
export default {
  props: ['titles'],
  components: {
    Items
  },
}
</script>

<style scoped>
  ul {
    list-style: none;
    margin: 0;
    padding: 0;
    width: 100%;
    height: 60px;
  }
</style>
