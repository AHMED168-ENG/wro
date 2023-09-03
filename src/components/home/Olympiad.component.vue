<template>
  <section class="olympiad">
    <div class="container">
      <div class="image">
        <img src="../../assets/nav3.png" alt="" />
      </div>
      <header>
        <h2><span>الأوليمبياد</span> العالمي للروبوت</h2>
        <p>
          هي منظمة عالمية غير ربحية عدد أعضائها أكثر من 90دولة، تهدف لإظهار
          إبداعات الشباب ومهاراتهم للفئة من8 إلى 19 عام وذلك عن طريق منافسات في
          الروبوت والذكاء الاصطناعي وتقام سنويًا بتحديات رياضية وتقنية مع طرح
          موضوع سنوي للابتكار في المشاكل التي تواجه العالم.
        </p>
        <p>
          وتتضمن هذه المسابقة عدة فئات ومنها مهام الروبوت البرمجية والتي سيتم
          العمل عليها من خلال محاكي افتراضي يقدم بيئة مليئة بالتحديات والاثارة
          وتعتمد على لغة برمجية بسيطة وسهلة<a href=""> بالكتل البرمجية</a>
        </p>
      </header>
      <div class="categorys">
        <div class="image">
          <img src="../../assets/image10.png" alt="" />
        </div>
        <div class="over">
          <div class="head">
            <h5><span>فئة</span> مهام الروبوت</h5>
            <h5>البرمجية</h5>
          </div>
          <p>
            هي فئة تهدف إلى تطوير المهارات التقنية من خلال برمجة الروبوت
            الافتراضي في بيئة رقمية تهتم بمجال الروبوت
            <a href="">والذكاء الاصطناعي تمكنهم</a>
            من التعلم والتحدي في بناء <a href="">الاستراتيجيات من</a> حلول
            المشكلات التقنية عن طريق برمجة الروبوت.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "OlympiadComponent",
};
</script>

<style lang="scss" scoped>
@import "../../scss/variables.scss";

.olympiad {
  background: $main-color;
  padding: 50px 0;
  .image {
    width: 32%;
    margin: 0 auto 25px;
    img {
      width: 100%;
    }
  }
  header {
    margin-bottom: 50px;
    text-align: center;
    h2 {
      span {
        color: $bink-color;
      }
      color: $green-color;
      font-size: 32px;
      font-weight: 700;
      margin-bottom: 35px;
    }
    p {
      a {
        color: $bink-color;
      }
      font-size: 22px;
      font-weight: 500;
      color: white;
      width: 78%;
      margin: 0 auto 20px;
    }
    p:last-of-type {
      margin-bottom: 80px;
    }
  }
  .categorys {
    background: $green-color;
    border-radius: 15px;
    position: relative;
    .image {
      position: absolute;
      right: 0;
      top: 0;
      width: 40%;
      height: 100%;
      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }
    .over {
      padding: 5px 20px 20px;
      .head {
        width: 250px;
        margin: -45px auto 20px;
        aspect-ratio: 1/0.7;
        flex-shrink: 0;
        background: url("../../assets/image7.png");
        background-size: cover;
        padding: 20px;
        h5 {
          color: white;
          font-size: 25px;
          text-align: center;
          font-weight: 700;
          span {
            color: $bink-color;
          }
        }
        h5:nth-of-type(1) {
          margin-bottom: 15px;
        }
      }
      p {
        color: white;
        font-weight: 400;
        width: 90%;
        margin: 0 auto 20px;
        font-size: 18px;
        a {
          color: $bink-color;
        }
      }
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
