<template>
  <div class="container">
   <!-- / {{myData}} -->
    <ul class="list-group">
      <li class="list-group-item" v-for="data in myData" :key="data">
           {{ myData.id }} - {{myData.name}}
      </li>
    </ul>

  </div>
</template>

<script>
import myData from '/src/data/myData'
export default {
  name: "MyTestApp",
   data() {
     return {
     myData
     }
   }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
