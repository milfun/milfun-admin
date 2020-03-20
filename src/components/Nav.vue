<template>
  <div class="navLeft">
    <div class="logo"><img src="../assets/a2.jpg"></div>
    <div class="items">
        <div class="item" v-for="item in items">
        <img src="../assets/a2.jpg"></div>
    </div>
    <div class="setting"><img class="img-40" src="../assets/a2.jpg"></div>
  </div>
</template>

<script>
export default {
  name: 'Nav',
  data () {
    return {
      items:['1','2','3','4','5']
    }
  },
  methods:{
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.navLeft{
  display: flex;
  flex-direction: column;
  position: absolute; top:0; left:0; width:100px;
  width:100px;
  height:100%;
  border-right: 1px solid #bbb;
  box-shadow: 1px 1px 50px rgba(0,0,0,.3);
}
.logo{flex: 2;padding-top: 20px;}
.logo img{
  width: 40px;
  height: 40px;
  border-radius: 50%;

}
.items{
  display: flex; flex: 8;
  flex-direction: column;
  align-items: center; }


.item{
  display: inline-flex;
  margin: 10px 0;
  border-radius: 10px;
  border: 1px solid #bbb;
  overflow: hidden;
}
.item img{width: 40px;height: 40px;border-radius: 10px;}
.img-40{
  width: 40px;
  height: 40px;
  border-radius: 10px;
}
.setting{display: flex;flex-direction: column;align-items: center;padding-bottom: 20px; justify-content: flex-end; flex: 2;margin-top: auto;}

</style>
