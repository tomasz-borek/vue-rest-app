<template>
  <div id="comments">
    <div id="comments-header">Komentarze:</div>
    <SingleComment 
    v-for="data in myJson" 
    :key="data.id"
    :data="data"></SingleComment>
  </div>
</template>

<script>
import json from "../data/data.json"
import SingleComment from "./SingleComment.vue"

export default {
  name: "HomePage",
  data() {
    return {
      myJson: json
    }
  },
  components: {
    SingleComment
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

#comments-header {
  border-top: 3px solid black; 
  border-bottom: 3px solid black;
  color: white;
  background-color: green;
  vertical-align: middle;
}

#comments {
  margin-left: 25%;
  width: 50%;
  border-left: 2px solid black;
  border-right: 2px solid black;
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
</style>
