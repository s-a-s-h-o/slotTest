<template>
  <div class="wrapper">
      <div class="head">
        <slot name="head"></slot>
      </div>

      <slot name="messageBox"></slot>
      <slot name="body"></slot>
      <slot name="footer"></slot>
  </div>
</template>

<script>
export default {

}
</script>

<style>
  .head{background: red;}
</style>
