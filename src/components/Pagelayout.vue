<template>
  <div class="primarylayout">
    <div class="header">
      <img src="../assets/logo.png" alt>
      <div class="user">
        <span class="user_name">User: Hkex</span>
        <span class="user_status">(Online)</span>
      </div>
    </div>
    <div class="content">
      <List></List>
    </div>
    <div class="footer">
      @2019 京备案号2399979 | 本系统由深圳金证股份北京人工智能分公司维护支持
    </div>
  </div>
</template>

<script>
import List from './List'
export default {
  components: {
    List
  }
}
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
}
.primarylayout {
  display: flex;
  flex-direction: column;
  width: 100vw;
  height: 100vh;
  min-height: 100vh;
}
.header {
  width: 100%;
  height: 74px;
  background: url("../assets/headerbackground.png");
  display: flex;
  align-items: center;
  justify-content: space-between;
  box-sizing: border-box;
  padding:0 36px;
}
.user {
  height: 20px;
  font-size: 14px;
  font-family: PingFangSC-Medium;
  font-weight: 500;
  color: rgba(255, 255, 255, 1);
  line-height: 20px;
}
.user_name {
  display: inline-block;
  width: 140px;
}
.user_status {
  display: inline-block;
}
.content {
  width: 100%;
  min-height: calc(100vh - 74px - 50px);
  box-sizing: border-box;
  flex-shrink: 0;
}
.footer {
    flex-shrink: 0;
    height: 50px;
    width: 100%;
    background: #10416c;
    font-size: 14px;
    font-family: PingFangSC-Medium;
    font-weight: 500;
    color: white;
    line-height: 50px;
    text-align: center;
    margin: 0 auto;
}
</style>
