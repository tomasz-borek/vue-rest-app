<template>
        <div>
          <div id="comment-index">#{{data.id}}</div>
          <div id="comment-title">{{data.title}}</div>
          <div id="comment-body">{{data.body}}</div>
        </div>
</template>

<script>
export default {
    name: "SingleComment",
    props: ['data'],
}
</script>

<style lang="scss">

#comment-index {
    font-weight: bold;
}

#comment-title {
    border-top: 1px solid black;
    padding-top: 5px;
    padding-bottom: 5px;
    background-color: #DDDDDD;
    font-weight: bold;
}

#comment-body {
    padding: 10px;
    border-bottom: 1px solid black;
    background-color: #EEEEEE;
}

</style>