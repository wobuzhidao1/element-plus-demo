<template>  
    <button class="button">{{ btn }}</button>
</template>

<script setup>
import { capitalize } from "@element-plus-demo/utils";
import { ref } from "vue";

const btn = ref(capitalize("FABCDEFG22"));
</script>

<style scoped>
.button {  
    color: #fff; 
    background-color: #409eff;  
    border-color: #409eff;  
    display: inline-block;  
    line-height: 1;  
    white-space: nowrap;  
    cursor: pointer;  
    text-align: center;  
    box-sizing: border-box;  
    outline: none;  
    margin: 0;  
    font-weight: 500; 
    padding: 12px 20px;  
    font-size: 14px;  
    border-radius: 4px;
}
</style>
  