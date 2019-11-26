<template>
  <div>
    <search />
    <swiper
      indicator-dots
      indicator-color="rgba(0,0,0,.5"
      indicator-active-color="#fff"
      autoplay
      interval="3000"
      circular
    >
      <a href>
        <swiper-item>
          <img src="/static/uploads/banner1.png" />
        </swiper-item>
      </a>
      <a href>
        <swiper-item>
          <img src="/static/uploads/banner2.png" />
        </swiper-item>
      </a>
      <a href>
        <swiper-item>
          <img src="/static/uploads/banner3.png" />
        </swiper-item>
      </a>
    </swiper>
    <div class="navs">
      <a href>
        <img src="/static/uploads/icon_index_nav_4@2x.png" alt />
      </a>
      <a href>
        <img src="/static/uploads/icon_index_nav_3@2x.png" alt />
      </a>
      <a href>
        <img src="/static/uploads/icon_index_nav_2@2x.png" alt />
      </a>
      <a href>
        <img src="/static/uploads/icon_index_nav_1@2x.png" alt />
      </a>
    </div>
    <div class="floors">
      <div class="floor">
        <div class="title">
          <img src="/static/uploads/pic_floor01_title.png" alt />
        </div>
        <div class="item">
          <a href>
            <img src="/static/uploads/pic_floor01_1@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor01_2@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor01_3@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor01_4@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor01_5@2x.png" alt />
          </a>
        </div>
      </div>
      <div class="floor">
        <div class="title">
          <img src="/static/uploads/pic_floor02_title.png" alt />
        </div>
        <div class="item">
          <a href>
            <img src="/static/uploads/pic_floor02_1@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor02_2@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor02_3@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor02_4@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor02_5@2x.png" alt />
          </a>
        </div>
      </div>
      <div class="floor">
        <div class="title">
          <img src="/static/uploads/pic_floor03_title.png" alt />
        </div>
        <div class="item">
          <a href>
            <img src="/static/uploads/pic_floor03_1@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor03_2@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor03_3@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor03_4@2x.png" alt />
          </a>
          <a href>
            <img src="/static/uploads/pic_floor03_5@2x.png" alt />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import search from "@/components/search";
export default {
  components: {
    search
  },
  data() {
    return {};
  },
  methods: {},

  created() {
    // let app = getApp()
  }
};
</script>

<style scoped lang="less">
swiper {
  width: 750rpx;
  height: 340rpx;
  img {
    width: 100%;
    height: 100%;
  }
}
.navs {
  display: flex;
  box-sizing: border-box;
  align-items: center;
  justify-content: space-between;
  padding: 0 35rpx;
  width: 750rpx;
  height: 192rpx;
  a {
    display: block;
    width: 128rpx;
    height: 140rpx;
    img {
      width: 100%;
      height: 100%;
    }
  }
}
.floors {
  width: 750rpx;
  .floor {
    .title {
      box-sizing: border-box;
      height: 110rpx;
      padding-top: 30rpx;
      img {
        width: 750rpx;
        height: 60rpx;
      }
    }
    .item {
      overflow: hidden;
      padding: 0rpx 16rpx;
      a {
        float: left;
        margin-right: 10rpx;
        img {
          width: 100%;
          height: 100%;
        }
      }
      a:first-child {
        width: 232rpx;
        height: 386rpx;
      }
      a:nth-child(2),
      a:nth-child(5) {
        width: 273rpx;
        height: 188rpx;
      }
      a:nth-child(3),
      a:nth-child(4) {
        width: 193rpx;
        height: 188rpx;
      }
      a:nth-child(3),
      a:nth-child(5) {
        margin-right: 0;
      }
      a:nth-child(n + 4) {
        margin-top: 10rpx;
      }
    }
  }
  .floor:first-child {
    .item {
      a:nth-child(n + 2) {
        width: 233rpx;
        height: 188rpx;
      }
    }
  }
}
</style>
