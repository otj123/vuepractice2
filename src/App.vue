<template>
  <div class="menu">
    <a v-for="items in menu" :key="items">{{items}}</a>
    <a v-for="(items,i) in menu" :key="items">{{items}} {{i}}</a>
    <a>products</a>
    <a>about</a>
  </div>
  <img alt="Vue logo" src="./assets/logo.png">
  <div>
    <h4>{{products[0]}}</h4>
    <p>50 만원</p>
  </div>
  <div>
    <h4>{{products[1]}} 원룸</h4>
    <p>xx 만원</p>
  </div>
</template>

<script>

export default {
  name: 'App',
  data(){
    return{
      menu : ["a", "b", "c"],
      products : ["원룸1", "원룸2", "원룸3"]
    }
  },
  components: {
  }
}
</script>

// document.getElementById().innerHTML = ?? 데이터 꽂는 곳 1

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.menu{
  background: darkblue;
  padding : 15px;
  border-radius : 5px;
}
.menu a{
  color: white;
  padding: 10px;
}
</style>
