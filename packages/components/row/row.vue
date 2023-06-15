<template>
    <div class="el-row">
      <slot></slot>
    </div>
</template>
  
<style scoped lang="scss">
  .el-row {
    display: flex;
    flex-wrap: wrap;
    position: relative;
    box-sizing: border-box;
  }
</style>