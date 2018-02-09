<template>
  <div class="layout-nav">
    <MenuItem name="1">
      <Icon type="ios-navigate"></Icon>
      Item 1
    </MenuItem>
    <MenuItem name="2">
      <Icon type="ios-keypad"></Icon>
      Item 2
    </MenuItem>
    <MenuItem name="3">
      <Icon type="ios-analytics"></Icon>
      Item 3
    </MenuItem>
    <MenuItem name="4">
      <Icon type="ios-paper"></Icon>
      Item 4
    </MenuItem>
  </div>
</template>

<script>
  export default {
    name: 'header'
  }
</script>

<style scoped>
  .layout-nav {
    width: 420px;
    margin: 0 auto;
    margin-right: 20px;
  }
</style>
