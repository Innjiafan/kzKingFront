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

    </section>
  </div>
</template>
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
    background: linear-gradient(90deg, #FF6C4A 0%, #FF7B62 100%);
  }
</style>