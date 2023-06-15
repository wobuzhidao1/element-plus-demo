<template>
    <div :class="{ [baseClassName]: true, [spanClassName]: true }">
      <slot></slot>
    </div>
</template>
<script setup>
  const props = defineProps(["span"]);
  
  function getSpan(propSpan) {
    if (typeof propSpan === "number") {
      const span = Math.ceil(Number(propSpan));
      if (span >= 1 && span <= 24) {
        return span;
      }
    }
    return 1;
  }
  
  const baseClassName = `baseClassName`; //基础样式
  const spanClassName = `col-${getSpan(props.span)}`; //
  </script>
  
  <style scoped lang="scss">
  $total-columns: 24; //列数
  $column-width: 100% / $total-columns; //每列的宽度
  
  .baseClassName {
    box-sizing: border-box;
  }
  
  @for $i from 1 through $total-columns {
    .col-#{$i} {
      width: ($column-width * $i);
      flex: 0 0 percentage((1 / $total-columns * $i));
    }
  }
  </style>