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
        </section>
      </div>
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
  }
</style>