<template>
  <section class="landing-page">
    <div class="over">
      <div class="image">
        <img src="../../assets/image10.png" alt="" />
      </div>
      <div class="content">
        <div class="images">
          <img src="../../assets/Frame.png" alt="" />
          <img src="../../assets/triangle.png" alt="" />
        </div>
        <header>
          <h2>فئة مهام</h2>
          <h2>الروبوت البرمجية</h2>
        </header>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "LandingPageComponent",
};
</script>

<style lang="scss" scoped>
.landing-page {
  overflow: hidden;
  position: relative;
  background-image: url("../../assets/landingPage.png");
  background-position: center center;
  background-size: cover;
  background-repeat: no-repeat;
  .over {
    padding: 0 20px;
    height: calc(100vh - 100px);
    position: relative;
    > .image {
      width: 70%;
      height: 67%;
      position: absolute;
      bottom: 30%;
      right: 15%;
      img {
        width: 100%;
        height: 100%;
      }
    }
    .content {
      position: absolute;
      width: 40%;
      top: 20%;
      left: 50%;
      transform: translateX(-50%);
      display: flex;
      flex-direction: column;
      align-items: center;
      header {
        position: relative;
        z-index: 10;
        h2 {
          font-size: 60px;
          font-weight: 700;
          text-align: center;
        }
        h2:nth-of-type(1) {
          color: #57b7aa;
          margin-bottom: 15px;
        }
        h2:nth-of-type(2) {
          color: #fff;
        }
      }
      .images {
        width: 35%;
        position: relative;
        img {
          width: 100%;
          height: 100%;
        }
        img:nth-of-type(2) {
          width: 90%;
          height: 90%;
        }
        img:nth-of-type(2) {
          position: absolute;
          bottom: -47%;
          left: -35%;
        }
      }
    }
  }
}

@media (max-width: 1500px) {
  nav .nav-wrapper .left {
    width: 30%;
  }
}
@media (max-width: 1300px) {
  .landing-page .over .content {
    width: 105%;
  }
}

@media (max-width: 1000px) {
  nav .nav-wrapper .left {
    width: 55%;
  }
}

@media (max-width: 700px) {
  .landing-page .over .content header h2:nth-of-type(1) {
    margin-bottom: 10px;
  }
  .landing-page .over .content {
    width: 116%;
  }
  .landing-page .over .content header h2 {
    font-size: 40px;
  }
}
@media (max-width: 400px) {
  .landing-page .over .content header h2:nth-of-type(1) {
    margin-bottom: 0px;
  }
  .landing-page .over .content {
    width: 116%;
  }
  .landing-page .over .content header h2 {
    font-size: 35px;
  }
}
</style>
