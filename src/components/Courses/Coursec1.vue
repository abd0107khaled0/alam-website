<template>
  <div class="coursec1 pt-16 mt-16">
    <v-container>
      <v-row>
        <v-col
          cols="12"
          lg="4"
          md="6"
          sm="6"
          class="pa-10"
          v-for="n in 3"
          :key="n.id"
        >
          <v-card>
            <v-card-title class="card_img">
              <img :src="require('@/assets/img/course.png')" alt=""
            /></v-card-title>
            <v-card-text class="card_title text-left pl-10">
              <h1 class="mt-5 mb-5">COURSE 1</h1>
              <p>DESCRIPTION AND SOME INFORMATION ABOUT COURSE</p>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "CourseC1",
};
</script>

<style lang="scss" scoped>
.coursec1 {
  .card_title {
    h1 {
      color: #2ca0e2;
      position: relative;
      opacity: 0.8;
      cursor: pointer;
      &::before {
        position: absolute;
        content: "";
        left: -20px;
        top: 10px;
        height: 50px;
        width: 5px;
        padding: 3px;
        border-radius: 4px;
        background: #2ca0e2;
      }
      &:hover {
        opacity: 1;
      }
    }
    p {
      color: #2ca0e2;
      font-weight: bold;
      font-size: 18px;
    }
  }
}
</style>
