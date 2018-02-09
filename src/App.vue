<template>
  <div id="app">
    <div class="layout">
      <Layout>
        <Header :style="{position: 'fixed', width: '100%'}">
          <Menu mode="horizontal" theme="dark" active-name="1">
            <div class="layout-logo"></div>
            <c-header></c-header>
          </Menu>
        </Header>
        <!--<div class="content-layout">-->
        <Content :style="{margin: '88px 20px 0', background: '#fff', minHeight: '100%'}">
          <router-view></router-view>
        </Content>
        <!--</div>-->
        <!--<Footer class="layout-footer-center">2011-2016 &copy; TalkingData</Footer>-->
      </Layout>
    </div>
  </div>
</template>

<script>
  import CHeader from '@/components/CHeader.vue'

  export default {
    name: 'App',
    components: {
      CHeader
    }
  }
</script>

<style lang="scss">
  #app {
    width: 100%;
    height: 100%;
  }

  .layout {
    width: 100%;
    height: 100%;
    border: 1px solid #d7dde4;
    background: #f5f7f9;
    position: relative;
    border-radius: 4px;
    overflow: hidden;
    .layout-logo {
      width: 100px;
      height: 30px;
      background: #5b6270;
      border-radius: 3px;
      float: left;
      position: relative;
      top: 15px;
      left: 20px;
    }
    .content-layout {
      /*height: calc(100% - 100px);*/
    }
    .layout-footer-center {
      text-align: center;
    }
  }
</style>
