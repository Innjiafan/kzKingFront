<template>
  <div class="container">
    <section class="banner">
      <div class="w1200">
        <section class="nav my-flex">
          <div class="logo-box my-flex">
            <img src="@/assets/images/icon/icon-logo.svg" alt="">
            <div class="r">
              <h4>快转王办公助手</h4>
              <p>高效易用  在线办公必备</p>
            </div>
          </div>
          <div class="menu">
            <ul>
              <li>首页</li>
              <li>PDF转换<span class="tri"></span></li>
              <li>CAD转换<span class="tri"></span></li>
              <li>语音识别<span class="tri"></span></li>
              <li>图文识别<span class="tri"></span></li>
              <li>我的</li>
            </ul>
          </div>
          <div class="login">登录</div>
        </section>
      </div>
    </section>
    <section class="carousel-container">
      <div class="w1200 carousel">
        <img class="img1" src="../assets/images/index/banner01.png" alt="">
        <img class="img2" src="../assets/images/index/banner02.png" alt="">
        <img class="img3" src="../assets/images/index/banner03.png" alt="">
        <h2>快转王 PDF 转换助手</h2>
        <h4>高质量识别，完美转换</h4>
        <p class="desc">支持 PDF 与 Word、PPT、Excel 等文件快速互转</p>
        <p class="desc">本地转换安全隐私保护，格式排版高保真，有效提升办公效率！</p>
        <button type="secondary">立即转换</button>
      </div>
    </section>
    <section class="func-container">
      <div class="w1200">
        <h4>在线转换</h4>
        <div class="func-panel">
          <dl class="func-item" v-for="(item,index) in func" :key="index">
            <dt>
              <img :src="imgUrl(index+1)" alt="">
            </dt>
            <dd>{{item.title}}</dd>
          </dl>
        </div>
      </div>
    </section>
    <section class="advan-container">
      
    </section>
  </div>
</template>
<script>
export default {
  data(){
    return {
      func:[{title:'PDF转Word',desc:'支持将PDF文件转换成Word文件'},
            {title:'PDF转Excel',desc:'支持将PDF文件转换成Excel文件'},
            {title:'PDF转PPT',desc:'支持将PDF文件转换成PPT演示文稿'},
            {title:'PDF转图片',desc:'支持将PDF文件转换成JPG等图片格式'},
            {title:'PDF压缩',desc:'支持压缩PDF文件的大小'},
            {title:'PDF合并',desc:'支持将多个PDF文件合并成一个PDF文件'},
            {title:'Word转PDF',desc:'支持将Word文件转换成PDF文件'},
            {title:'Excel转PDF',desc:'支持将Excel文件转换成PDF文件'},
            {title:'PPT转PDF',desc:'支持将PDF文件转换成Excel文件'},
            {title:'图片转PDF',desc:'支持将JPG等图片格式转换成PDF文件'},
            {title:'语音转换',desc:'支持多国文本进行语言转换'},
            {title:'更多功能',desc:'PDF转换助手支持18项PDF主流功能，全面满足您的日常需求'}]
    }
  },
  computed:{
    imgUrl(){
      return function(index){
        return require('../assets/images/index/icon_func'+index+'.svg')
      }
    }
  }
}
</script>
<style lang="scss" scoped>
  .w1200{
    width: 1260px;
    margin: 0 auto;
  }
  .banner{
    width:100%;
    height: 70px;
    background-color: #fff;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 2;
  }
  .nav{
    display: flex;
    align-items: center;
    height: 70px;
    .logo-box{
      flex: 0 0 180px;
      img{
        width: 42px;
        height: 42px;
        margin-right: 10px;
      }
      h4{
        font-size: 18px;
        font-weight: bold;
        color: #1A1A1A;
        line-height: 18px;
        margin-bottom: 2px;
      }
      p{
        color: #BBBBBB;
      }
    }
    .menu{
      flex: 1;
      padding-left: 144px;
      box-sizing: border-box;
      ul{
        display: flex;
        align-items: center;
      }
      ul>li{
        height: 100%;
        margin-right: 36px;
        color:#333;
        font-size: 14px;
        display:flex;
        align-items:center
        
      }
      .tri{
        display: inline-block;
        content:'';
        width: 0;
        height: 0;
        border-left: 4px solid transparent;
        border-right: 4px solid transparent;
        border-top: 6px solid #000;
        margin-left: 6px;
      }
    }
    .login{
      flex: 0 0 105px;
      width: 105px;
      height: 40px;
      line-height: 40px;
      text-align: center;
      background: #FF6C4A;
      border-radius: 2px;
      color: #fff;
    }
  }
  .carousel-container{
    width: 100%;
    height: 520px;
    margin-top: 70px;
    background: linear-gradient(90deg, #FF6C4A 0%, #FF7B62 100%);
    .carousel{
      position: relative;
      height: 100%;
      h2{
        font-size: 44px;
        font-weight: bold;
        padding-top: 70px;
        color: #fff;
      }
      h4{
        font-size: 28px;
        font-weight: 400;
        color: #fff;
        margin-bottom: 20px;
        margin-top: 43px;
      }
      .desc{
        color: #FFFFFF;
        font-size: 18px;
        line-height: 26px;
        margin-bottom: 33px;
      }
      button[type='secondary']{
        width: 229px;
        height: 66px;
        background: #FFFFFF;
        border-radius: 6px;
        line-height: 66px;
        text-align: center;
        cursor: pointer;
        border: none;
        color: #FF7B62;
        font-size: 20px;
      }
      .img1{
        position: absolute;
        bottom: 0;
        left: 217px;
        width: 340px;
        height: 110px;
        z-index: 1;
      }
      .img2{
        position: absolute;
        right:72px;
        top: 0;
        width: 556px;
        height: 357px;
      }
      .img3{
        position: absolute;
        right:0;
        top: 92px;
        width: 646px;
        height: 375px;
      }
    }
  }
  .func-container{
    width: 100%;
    height: 576px;
    background: #F8F8F8;
    h4{
      color: #333333;
      font-size: 36px;
      font-weight: 400;
      margin-bottom: 71px;
      padding-top: 70px;
      width: 100%;
      text-align: center;
    }
    .func-panel{
      width: 100%;
      height: 388px;
      background: #FFFFFF;
      box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1);
      border-radius: 6px;
      display: flex;
      align-items: center;
      flex-wrap: wrap;
      .func-item{
        width: 210px;
        height: 194px;
        background: #FFFFFF;
        display: flex;
        align-items: center;
        flex-direction: column;
        justify-content: center;
        dt{
          img{
            width: 43px;
            height: 50px;
            margin-bottom: 38px;
          }
        }
        dd{
          color: #333333;
          font-weight: bold;
          font-size: 18px;
        }
      }
      .func-item:hover{
        background: linear-gradient(180deg, #FF6C4A 0%, #FF7B62 100%);
        dd{
          color: #fff;
        }
      }
    }
  }
</style>