<script setup>
import { Button, Row, Col } from "@element-plus-demo/components";
</script>

<template>
  <div class="container">
    <Button style="margin-bottom: 24px"></Button>
    <Row>
      <Col class="gird" :span="24">col-24</Col>
    </Row>
    <Row>
      <Col class="gird" :span="12">col-12</Col>
      <Col class="gird-dark" :span="12">col-12</Col>
    </Row>
    <Row>
      <Col class="gird" :span="8">col-8</Col>
      <Col class="gird-dark" :span="8">col-8</Col>
      <Col class="gird" :span="8">col-8</Col>
    </Row>
    <Row>
      <Col class="gird" :span="6">col-6</Col>
      <Col class="gird-dark" :span="6">col-6</Col>
      <Col class="gird" :span="6">col-6</Col>
      <Col class="gird-dark" :span="6">col-6</Col>
    </Row>
  </div>
</template>

<style scoped lang="scss">
.container {
  width: 960px;
  margin: 0 auto;
}
.gird {
  background: #8cbfe6;
  border: 1px #8cbfe6 solid;
  margin-bottom: 10px;
  height: 50px;
  color: #ffffff;
  font-size: 18px;
  text-align: center;
  line-height: 50px;
}
.gird-dark {
  background: #068aed;
  border: 1px #068aed solid;
  margin-bottom: 10px;
  height: 50px;
  color: #ffffff;
  font-size: 18px;
  text-align: center;
  line-height: 50px;
}
</style>