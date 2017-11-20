<template>
  <div class="layout">
    <router-view></router-view>
  </div>
</template>
<script>
  export default {}
</script>
<style lang="scss">
  @import "assets/sass/index";

  $copy-right-text-color: #9ea7b4;
  $full-height: 100%;
  $page-background-color: #f5f7f9;
  $content-background-color: #fff;
  .layout {
    border: 1px solid #d7dde4;
    background: $page-background-color;
    position: relative;
    height: $full-height;
    width: 100%;
    .layout-breadcrumb {
      padding: 10px 15px 0;
      & > * {
        display: inline-block;
      }
    }

    .layout-logo {
      border-radius: 3px;
      float: left;
      margin-left: 20px;
      span {
        font-size: 16px;
        color: #fff;
      }
      .ivu-icon {
        color: #fff;
      }
    }

    .layout-nav {
      width: 420px;
      margin: 0 auto;
    }

    .layout-breadcrumb {
      padding: 10px 15px 0;
      .ivu-btn {
        padding-left: 5px;
      }
    }

    .layout-content {
      min-height: 200px;
      margin: 15px;
      overflow: hidden;
      height: calc(100% - 138px);
      background: $content-background-color;
      border-radius: 4px;
      .ivu-row, .ivu-col, .ivu-menu {
        height: $full-height;
      }
    }

    .layout-content-main {
      padding: 10px 15px 0;
      height: calc(100% - 61px);
    }

    .layout-copy {
      text-align: center;
      padding: 10px 0 20px;
      color: $copy-right-text-color;
    }
  }
</style>
