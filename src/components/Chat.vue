<template>
  <div >
		<div class="milfun-chat-head">
			<div class="milfun-im-info">
				<p>纸飞机</p>
				<input class="milfun-im-remark" placeholder="编辑签名" value="在深邃的编码世界，做一枚轻盈的纸飞机">
			</div>
			<div class="milfun-chat-username"></div>
		</div>
		<div class="milfun-chat-body">
			<div class="milfun-chat-msg">
				
			</div>
		</div>
		<div class="milfun-chat-foot">
			
			<div class="milfun-chat-tool">
				<span>😁</span>
				<span>🎞</span>
				<span>🚟</span>
				<span>🎧</span>
				<span>🎼</span>
			</div>
		</div>
	</div>
</template>

<script>
export default {
  name: 'Chat',
  data () {
    return {
      items:['1','2','3','4','5']
    }
  },
  methods:{
  }
}
</script>


<style scoped>
	.milfun-chat, .milfun-im {
  display: flex;
  flex-direction: column;
  z-index: 19891017;
  width: 500px;
  height: 420px;
  background-color: white;
  border-radius: 50%;
  position: absolute;
  border-radius: 2px;
  box-shadow: 1px 1px 50px rgba(0, 0, 0, 0.3);
  box-sizing: border-box;
  overflow: hidden; }
  .milfun-chat .milfun-chat-head, .milfun-im .milfun-chat-head {
    display: inline-flex;
    align-items: center;
    height: 80px;
    background-color: rgba(245, 245, 245, 0.7); }
    .milfun-chat .milfun-chat-head .milfun-chat-headimg img, .milfun-im .milfun-chat-head .milfun-chat-headimg img {
      position: absolute;
      left: 0;
      top: 0;
      width: 50px;
      height: 50px;
      border-radius: 100%; }
  .milfun-chat .milfun-chat-body, .milfun-im .milfun-chat-body {
    height: 300px; }
  .milfun-chat .milfun-chat-foot, .milfun-im .milfun-chat-foot {
    background-color: rgba(245, 245, 245, 0.7); }
    .milfun-chat .milfun-chat-foot .milfun-chat-tool, .milfun-im .milfun-chat-foot .milfun-chat-tool {
      position: relative;
      padding: 0 8px;
      height: 38px;
      line-height: 38px;
      font-size: 0; }
      .milfun-chat .milfun-chat-foot .milfun-chat-tool span, .milfun-im .milfun-chat-foot .milfun-chat-tool span {
        position: relative;
        margin: 0 10px;
        display: inline-block;
        vertical-align: top;
        font-size: 18px;
        cursor: pointer; }
      .milfun-chat .milfun-chat-foot .milfun-chat-tool .milfun-chat-log, .milfun-im .milfun-chat-foot .milfun-chat-tool .milfun-chat-log {
        position: absolute;
        right: 5px;
        font-size: 14px; }
    .milfun-chat .milfun-chat-foot .milfun-chat-input, .milfun-im .milfun-chat-foot .milfun-chat-input {
      margin-left: 10px; }
      .milfun-chat .milfun-chat-foot .milfun-chat-input textarea, .milfun-im .milfun-chat-foot .milfun-chat-input textarea {
        display: block;
        width: 100%;
        padding: 5px 0 0;
        height: 68px;
        line-height: 20px;
        border: none;
        overflow: auto;
        resize: none;
        background: 0 0; }
    .milfun-chat .milfun-chat-foot .milfun-chat-button, .milfun-im .milfun-chat-foot .milfun-chat-button {
      height: 50px;
      text-align: right;
      padding: 5px 10px;
      box-sizing: border-box; }
      .milfun-chat .milfun-chat-foot .milfun-chat-button span, .milfun-im .milfun-chat-foot .milfun-chat-button span {
        display: inline-block;
        vertical-align: top;
        font-size: 14px;
        line-height: 32px;
        margin-left: 5px;
        padding: 0 20px;
        background-color: #5FB878;
        color: #fff;
        border-radius: 3px; }
.milfun-im {
  display: flex;
  flex-direction: column;
  z-index: 19891016;
  width: 260px;
  height: auto;
  border-radius: 50%;
  position: absolute;
  right: 0;
  bottom: 0;
  border-radius: 2px;
  box-shadow: 1px 1px 50px rgba(0, 0, 0, 0.3);
  background-image: url(https://res.layui.com/layui/dist/css/modules/layim/skin/3.jpg);
  box-sizing: border-box;
  overflow: hidden; }
  .milfun-im .milfun-chat-head {
    display: inline-flex;
    align-items: center;
    padding: 0 10px;
    height: 80px;
    background-color: rgba(245, 245, 245, 0.7);
    box-sizing: border-box;
    overflow: hidden; }
    .milfun-im .milfun-chat-head .milfun-im-info {
      width: 100%; }
      .milfun-im .milfun-chat-head .milfun-im-info .milfun-im-remark {
        left: -6px;
        display: block;
        width: 100%;
        border: 1px solid transparent;
        margin-top: 8px;
        height: 26px;
        line-height: 26px;
        background: 0 0;
        border-radius: 2px; }
  .milfun-im .milfun-chat-foot {
    position: absolute;
    bottom: 0;
    width: 100%; }

</style>