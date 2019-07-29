<template>
<div>
  <div class="head">
      <i class="sou" @click="sousuo()"></i>
      <input class="in1" type="text" placeholder="请输入感兴趣的关键字和发布者昵称" @click="dofn()"/>
  </div>
</div>
</template>
<script>
export default {
  methods :{
    dofn(){
      const url='../community/main'
      wx.navigateTo({url});
    }
  },
}
</script>
<style>
.head{
        width: 364px;
        margin-top: 5px;
        margin-left: 5px;
        height: 35px;
        background-color: rgba(30, 31, 31, 0.164);
        position: relative;
        border-radius: 20px;
    }
    .in1{
        margin-left:30px; 
        width: 320px;
        height: 35px;
        float: left;
        background-color:transparent;
    }
    .sou{
        background: url(../../../static/images/sou1.png) ;
        margin-top:10px; 
        margin-left: 10px;
        width: 16px;
        height: 16px;
        position: absolute;
    }
</style>
