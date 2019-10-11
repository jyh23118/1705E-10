<template>
  <div id="app">  
    <router-view/>
    <div id="nav">
      <router-link to="/" tag="span">首页</router-link>
      <router-link to="/about" tag="span">我的</router-link>
    </div>
  </div>
</template>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  list-style: none;
  box-sizing: border-box;
}
html,body,#app{
  width: 100%;
  height: 100%;
}
#app {
  display: flex;
  flex-direction: column;
  #nav{
    width: 100%;
    line-height: 60px;
    display: flex;
    span{
      flex: 1;
      text-align: center;
      &.router-link-exact-active{
         color: seagreen;
      }
    }
  }
}
</style>
