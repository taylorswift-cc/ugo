<template>
  <div class="search">
    <div class="search_box">
      <input type="text" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="less" scoped>
.search {
  width: 750rpx;
  height: 110rpx;
  background-color: #ea4451;
  box-sizing: border-box;
  padding: 20rpx 30rpx;
  .search_box {
    height: 60rpx;
    position: relative;
    &::after {
      content: "搜索";
      display: block;
      color: #c2c2c2;
      font-size: 24rpx;
      height: 32rpx;
      padding-left: 60rpx;
      line-height: 32rpx;
      position: absolute;
      left: 50%;
      top: 50%;
      transform: translate(-50%, -50%);
      background: url(https://ugo2.oss-cn-hangzhou.aliyuncs.com/images/icon_search%402x.png)
        no-repeat;
      background-size: auto 32rpx;
    }
    input {
      width: 100%;
      height: 100%;
      border-radius: 8rpx;
      background-color: #fff;
    }
  }
}
</style>