<template>
  <div class="hello">

    <!--img width="20%" src="../assets/allyisonlogo.png"-->
    <h1>aas</h1>
a
    <button v-for="id in categories" type="button" class="btn btn-primary">
      <span class="hotkey">{{id[0]}}</span>
      {{id[1]}}
    </button>

    <Video title="video 1" class="allyvideo"/>
    <Video title="video 2" class="allyvideo"/>
    <Video title="video 3" class="allyvideo"/>
    <Video title="video 4" class="allyvideo"/>
    <Video title="video 5" class="allyvideo"/>

  </div>
</template>

<script>
import Video from "./Video";

export default {
  name: "HelloWorld",
  components: {
    Video
  },
  data: function() {
    return {
      categories: [["S", "soccer"], ["B", "baseball"], ["H", "hockey"]],
      vids: [1]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.allyvideo{
  float:left;
}

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

.hotkey {
  border: #222 1px solid;
  padding: 0 3px 0 3px;
}
</style>
