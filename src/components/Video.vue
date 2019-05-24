<template>
  <div class="video">
    <img width="5%" src="../assets/logo.png">
    <span class="tag" v-for="i in 3">#{{i}}</span>
  </div>
</template>

<script>
export default {
  name: "Video",
  props:['title'],
  data: function() {
    return {
      vids: [1]
    };
  }
};
</script>

<style scope>

.tag{ border:black 1px;}

</style>