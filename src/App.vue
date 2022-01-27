<template>
  <div id="app">
    <div>
      <el-carousel :interval="4000" type="card" height="200px">
        <el-carousel-item v-for="item in imagebox" :key="item.id">
          <img :src="item.idView" class="image">
        </el-carousel-item>
      </el-carousel>
      
    </div>
    
    <div>
      <img alt="Vue logo" width="70%" src="./assets/guohua4.jpg">
    </div>

      <div>
        <button  class = "button green"> 点击领取 </button>
      </div>

    <div>
      <img alt="Vue logo" width="70%" src="./assets/guohua3.jpg">
    </div>

      <div>
        <button  class = "button green"> 点击领取 </button>
      </div>
    
    <div>
      <img alt="Vue logo" width="70%" src="./assets/guohua2.jpg">
    </div>

      <div>
        <button  class = "button green"> 点击领取 </button>
      </div>

    <div>
      <img alt="Vue logo" width="70%" src="./assets/guohua1.jpg">
    </div>

      <div>
        <button  class = "button green"> 点击领取 </button>
      </div>

  </div>

  

  
</template>

<script>

export default {
  name: 'App',
  components: {
    
  },
  data(){
      return {
        imagebox:[{id:0,idView:require('./assets/guohua3.jpg')},
        {id:1,idView:require('./assets/guohua4.jpg')},
        {id:2,idView:require('./assets/guohua2.jpg')},
        {id:2,idView:require('./assets/guohua1.jpg')}
        //imagebox是assets下一个放图片的文件夹
        ]
      }
    }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.button {
 display: inline-block;
 zoom: 1; /* zoom and *display = ie7 hack for display:inline-block */
 *display: inline;
 vertical-align: baseline;
 margin: 0 2px;
 outline: none;
 cursor: pointer;
 text-align: center;
 text-decoration: none;
 font: 14px/100% Arial, Helvetica, sans-serif;
 padding: .5em 2em .55em;
 text-shadow: 0 1px 1px rgba(0,0,0,.3);
 -webkit-border-radius: .5em; 
 -moz-border-radius: .5em;
 border-radius: .5em;
 -webkit-box-shadow: 0 1px 2px rgba(0,0,0,.2);
 -moz-box-shadow: 0 1px 2px rgba(0,0,0,.2);
 box-shadow: 0 1px 2px rgba(0,0,0,.2);
}

.green {
 color: #e8f0de;
 border: solid 1px #426118;
 background: #42b983;
 background: -webkit-gradient(linear, left top, left bottom, from(#7db72f), to(#4e7d0e));
 background: -moz-linear-gradient(top,  #7db72f,  #4e7d0e);
 filter:  progid:DXImageTransform.Microsoft.gradient(startColorstr='#7db72f', endColorstr='#4e7d0e');
}

</style>
<style>
   .el-carousel__item h3 {
      color: #475669;
      font-size: 14px;
      opacity: 0.75;
      line-height: 200px;
      margin: 0;
    }

    .el-carousel__item:nth-child(2n) {
      background-color: #99a9bf;
    }

    .el-carousel__item:nth-child(2n+1) {
      background-color: #d3dce6;
    }
    img{
     /*设置图片宽度和浏览器宽度一致*/
      width:100%;
      height:inherit;
    }
</style>