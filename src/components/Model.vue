<template>
   <div class="model">
    <div class="md-modal modal-msg md-modal-transition md-show">
      <div class="md-modal-inner">
        <div class="md-top">
          <button class="md-close">关闭</button>
        </div>
        <div class="md-content">
          <div class="confirm-tips">
            <!-- <p slot="message">?</p> -->
            <slot name="message"></slot>
          </div>
          <div class="btn-wrap">
            <slot name="btnGroup"></slot>
          </div>
        </div>
      </div>
    </div>
    <div class="md-overlay"></div>
  </div>
</template>

<script>
export default {
  name: 'model',
  props:['mdShow']
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
