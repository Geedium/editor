<template>
  <div class="box">
    <div class="toolbar">
      <button>B</button>
      <button>U</button>
      <button>I</button>
    </div>
    <div class="viewport">
      <p class="viewport--p">⠀</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Editor",
};
</script>

<style scoped>
.box {
  box-shadow: 1px 2px 5px #c6c6c6;
  min-height: 150px;
  display: inline-block;
  min-width: 400px;
  overflow: hidden;
}
.toolbar {
  background: #fbfbfb;
  min-height: 32px;
  max-height: 40px;
  box-shadow: 0px 1px 3px 0px #e6e6e6;
  display: flex;
  flex-wrap: wrap;
  padding: 4px;
}
.toolbar button {
  width: 32px;
  height: 32px;
}
.viewport {
  position: absolute;
  left: 0;
  right: 0;
  bottom: 0;
  top: 40px;
  text-align: left;
  overflow-y: scroll;
  overflow-wrap: break-word;
}
.viewport:hover {
  cursor: text;
}
.viewport--p {
  display: inline;
}
</style>
