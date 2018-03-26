<template>
  <div id="app">
    <div class="header">
      <router-link tag="div" to="/index" class="to-index">
        <i>Wepost</i>
      </router-link>
      <div class="linkbox">
        <router-link tag="div" to="/index" class="link">
          <span>Wepost</span>
        </router-link>
        <router-link tag="div" to="/index" class="link">
          <span>Wepost</span>
        </router-link>
        <router-link tag="div" to="/index" class="link">
          <span>Wepost</span>
        </router-link>
      </div>

    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style  scoped lang="less" rel="stylesheet/less">
  @import "./assets/less/index.less";
  @media screen and (min-width:960px) and (max-width:1200px){
    .to-index{
      font-size: @font-size-md-5!important;
    }
  }
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  .header{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    height:5rem;
    line-height: 5rem;
    background-color: aliceblue;
    //color: #fff;

    .to-index{
      font-size: @font-size-large-5;
      margin-left: 5rem;
    }
    .linkbox{
      display: flex;
      flex-direction: row;
      justify-content: left;
      .link{
        font-size: @font-size-large-4;
        margin: 0 3rem;
      }
    }
  }
}
</style>
