<template>
  <div class="video">
    <img width="5%" src="../assets/logo.png">
    <div >
      <span class="tag" v-for="i in 3">#{{i}}</span>
    </div>
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

.tag{ 

  padding:0 2px 0 2px;
  margin-right:3px;
  border:black solid 1px;
  border-radius: 4px;
}

</style>