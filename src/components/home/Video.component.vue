<template>
  <section class="video">
    <div class="container">
      <header>
        <h4>للتعرف على المسابقة</h4>
      </header>
      <div class="video_wrapper">
        <video
          autoplay
          controls
          loop
          muted
          src="../../assets/video.mp4"
        ></video>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "VideoComponent",
};
</script>

<style lang="scss" scoped>
@import "../../scss/variables.scss";

.video {
  background: $main-color;
  padding: 50px 0;

  header {
    background: url("../../assets/image6.png");
    background-size: cover;
    width: 300px;
    padding: 20px;
    margin-bottom: 20px;
    h4 {
      color: $green-color;
    }
  }
  .video_wrapper {
    width: 100%;
    aspect-ratio: 1/0.6;
    width: 80%;
    margin: auto;
    video {
      object-fit: fill;
      width: 100%;
      height: 100%;
      border-radius: 25px;
    }
  }
}

@media (max-width: 1500px) {
}
@media (max-width: 1300px) {
  .olympiad header p {
    font-size: 20px;
    font-weight: 500;
    color: white;
    width: 90%;
    margin: 0 auto 20px;
  }
}

@media (max-width: 1000px) {
  .olympiad header p {
    font-size: 16px;
    font-weight: 500;
    color: white;
    width: 90%;
    margin: 0 auto 20px;
  }
  .video .video_wrapper {
    width: 100%;
  }
  .olympiad .categorys .over .head h5 {
    font-size: 20px;
  }
  .olympiad .categorys .over .head {
    width: 224px;
  }
  .olympiad .categorys .over p {
    font-size: 16px;
    width: 95%;
  }
  .olympiad .image {
    width: 40%;
  }
}

@media (max-width: 700px) {
  .olympiad header p {
    font-size: 16px;
    width: 100%;
  }
  .olympiad .categorys .over .head h5 {
    font-size: 20px;
  }
  .olympiad .categorys .over .head {
    width: 224px;
  }
  .olympiad .categorys .over p {
    font-size: 16px;
    width: 100%;
  }
}
@media (max-width: 400px) {
}
</style>
