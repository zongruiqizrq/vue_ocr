<template>
  <div class='content'>
    <div class='compoy'>
      <span class='title com-title'>Company's name</span>
      <el-input class='input' placeholder='请输入内容'></el-input>
      <span class='title status-title'>Status</span>
      <el-select class='select-box' v-model='value' placeholder='请选择'>
        <el-option
          v-for='item in options'
          :key='item.value'
          :label='item.label'
          :value='item.value'
        ></el-option>
      </el-select>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      options: [
        {
          value: '选项1',
          label: '黄金糕'
        },
        {
          value: '选项2',
          label: '双皮奶'
        },
        {
          value: '选项3',
          label: '蚵仔煎'
        },
        {
          value: '选项4',
          label: '龙须面'
        },
        {
          value: '选项5',
          label: '北京烤鸭'
        }
      ],
      value: ''
    }
  }
}
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
}
.content {
  width: 100%;
  height: 100%;
  padding: 20px 10%;
}
.compoy {
  display: flex;
  align-items: center;
}
.title {
  height: 28px;
  font-size: 14px;
  font-family: Arial-BoldMT;
  font-weight: normal;
  color: rgba(16, 65, 108, 1);
  line-height: 38px;
  text-align: center;
}
.com-title{
    width: 116px;
    flex-shrink: 0;
    margin-right: 10px;
}
.input{
    height:28px;
    background:rgba(255,255,255,1);
    border-radius:4px;
    border:1px solid rgba(222,224,226,1);
    margin-right:20px;
}
.status-title{
    margin-right: 10px;
    width: 43px;
    flex-shrink: 0;
}
.select-box{
    height:28px;
    background:rgba(255,255,255,1);
    border-radius:4px;
    border:1px solid rgba(222,224,226,1);
}
</style>
