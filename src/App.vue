<template>
  <div>
    <NavbarComponent></NavbarComponent>
    <LandingPageComponent></LandingPageComponent>
    <OlympiadComponent></OlympiadComponent>
    <VideoComponent></VideoComponent>
    <AgeCategoriesComponent></AgeCategoriesComponent>
  </div>
</template>

<script>
import NavbarComponent from "@/components/layouts/Navbare.component.vue";
import LandingPageComponent from "@/components/home/LandingPage.vue";
import OlympiadComponent from "@/components/home/Olympiad.component.vue";
import AgeCategoriesComponent from "@/components/home/AgeCategories.component.vue";
import VideoComponent from "@/components/home/Video.component.vue";
export default {
  name: "App",
  components: {
    NavbarComponent,
    LandingPageComponent,
    OlympiadComponent,
    VideoComponent,
    AgeCategoriesComponent,
  },
};
</script>

<style scope lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;500;600;700;800;900&display=swap");
body {
  overflow-x: hidden !important;
  padding-top: 100px;
}
* {
  direction: rtl;
  font-family: "Cairo";
}

.container {
  display: block !important;
}

@media (min-width: 576px) {
  .container,
  .container-lg,
  .container-md,
  .container-sm,
  .container-xl,
  .container-xxl {
    max-width: 85%;
  }
}
@media (min-width: 768px) {
  .container,
  .container-lg,
  .container-md,
  .container-sm,
  .container-xl,
  .container-xxl {
    max-width: 90% !important;
  }
}

@media (min-width: 1400px) {
  .container,
  .container-lg,
  .container-md,
  .container-sm,
  .container-xl,
  .container-xxl {
    max-width: 90% !important;
  }
}
* a {
  text-decoration: none;
}
ul {
  margin: 0;
  padding: 0;
}
.row {
  margin: 0 !important;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  margin: 0;
}
body::-webkit-scrollbar {
  width: 5px;
}

body::-webkit-scrollbar-track {
  box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
}

body::-webkit-scrollbar-thumb {
  background-color: #57b7aa;
  outline: 1px solid slategrey;
}
</style>
