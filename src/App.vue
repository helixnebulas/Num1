<template>
  <div id="app">
    <h1><strong> Общее состояние: </strong>
    <span class="badge bg-warning text-dark p-2">70%</span> </h1>
    
    <ul class= "list-group p-4 align-items-center" >
      <li id="test" class="list-group-item d-flex justify-content-between align-items-center" v-for="t in title" :key="t.status">
    <div> {{t.title}} </div>
    <span class="badge bg-success rounded-pill">1</span>
  </li>
  </ul>
  <button id="buttons" type="button" class="btn btn-outline-dark">Сделать что-то</button>
  <button type="button" class="btn btn-outline-dark">Сделать что-то ещё</button>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {

  },

  data() {
    return{
    title: [
      { title: "Загруженность аудиторий", status: 1},
      { title: "Пожелания преподавателей", status: 2},
      { title: "Физкультура", status: 3},
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
#test {
  width: 50%;
  height: 60px;
}
#buttons
{
  margin-right: 60px;
}
</style>
