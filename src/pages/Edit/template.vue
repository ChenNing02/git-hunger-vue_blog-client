<template>
  <div id="edit">
    <div class="edit-main">
      <h2>编辑文章</h2>
      <h3>文章标题<span class="msg">( 限30个字 )</span></h3>
      <el-input placeholder="请输入文章标题" v-model="title"></el-input>
      <h3>内容简介<span class="msg">( 限30个字 )</span></h3>
      <el-input type="textarea" :autosize="{ minRows: 2, maxRows: 10}" placeholder="请输入文章简介" v-model="description"></el-input>
      <h3>文章内容<span class="msg">( 限30个字 )</span></h3>
      <el-input type="textarea" :autosize="{ minRows: 6, maxRows: 10}" placeholder="请输入文章内容" v-model="content"></el-input>
      <div>
        <el-switch v-model="atIndex" active-color="#409EFF" active-text="在首页展示"></el-switch>
      </div>
      <el-button size="medium" type="primary" plain @click="onEdit">确定</el-button>
    </div>
  </div>
</template>

<script src="./template.js"></script>
<style lang="less" src="./template.less"></style>
