<template>
  <div id="app">
    <h1 ><strong> Общий статус: </strong> 
    <Percent/>
    </h1>
    <hr>
    <ListItems
      v-bind:titles="titles"
    />
  </div>
</template>

<script>
import ListItems from '@/components/ListItems'
import Percent from '@/components/Percent'
export default {
  name: 'App',
  components: {
    ListItems, Percent
  },

  data() {
    return{
    titles: [
      { id: 1, title: "Загруженность фонда", percent: 55},
      { id: 2, title: "Магистры разбиты", percent: 24},
      { id: 3, title: "Лекции магистров", percent: 15},
    ]
  }
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #050505;
  margin-top: 60px;
}
</style>
