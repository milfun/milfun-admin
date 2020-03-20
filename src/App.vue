<template>
  <div id="app">
    <Nav/>
    <div class="content">
        <div class="user">
            <span>查找</span>
            <span>消息</span>
            <img src="./assets/a1.jpg">
            <span>MilFun</span>
        </div>
        <div class="main">
            <div class="main-info">s</div>
            <div class="main-chat">
              <Chat />
            </div>
        </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Nav from './components/Nav'
import Chat from './components/Chat'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Nav,
    Chat
  }
}
</script>

<style>
body{
  margin: 0;
}
#app {
  display: flex;
  flex-direction: row;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
}
.content{
  display: inline-flex;
  justify-content: flex-end;
  flex-direction: column;
  background: purple;
  width: 100%;
  height: 100%;
  margin-left: 100px; background: #f0f;
}
.user{
  display: flex;
  justify-content: flex-end;
  align-items: center;
  height: 60px;
}
.user img{
  width: 30px;
  height: 30px;
  border-radius: 50%;
}
.user span{
  padding: 0 10px;
}
.main{
  display: flex;
  flex-direction: row;
  height: 100%;
  padding: 10px;
  background: #000;
  box-sizing: border-box;
  overflow: hidden;
}
.main-info{
  width: 100%;
  padding: 10px;
  background: #65a65c;
}

.main-chat{
  width: 400px;
  margin-left: 20px;
  background: #fff;
}
</style>
