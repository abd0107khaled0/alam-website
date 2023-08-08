<template>
  <div class="homec2">
    <v-container>
      <h1 color="white" class="mb-16 text-left">
        WHY <br />
        CEMcourses?
      </h1>
      <v-row>
        <v-col
          cols="12"
          lg="4"
          md="6"
          sm="12"
          xs="12"
          v-for="n in status"
          :key="n.id"
          class="card_for"
        >
          <v-card
            class="pa-10 card text-left"
            rounded="xl"
            style="background: #2ca0e2"
          >
            <v-card-title>
              <v-icon>mdi-account</v-icon>
            </v-card-title>
            <v-card-text>
              <span> {{ n.name }} </span>
              <p class="mt-2 mb-10">
                {{ n.p }}
              </p>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "HomeC3",
  data() {
    return {
      status: [
        {
          name: "Value",
          p: "High-quality courses at competitive prices",
          icon: "",
        },
        {
          name: "Quality",
          p: "Courses designed by experienced Chemistry professionals",
          icon: "",
        },
        {
          name: "Convenience",
          p: "Learn at your own pace, anytime, anywhere",
          icon: "",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.homec2 {
  background: #14365d;
  padding: 90px 0;
  h1 {
    color: white;
    font-size: calc(20px + 2vw);
  }
  .card_for:nth-of-type(even) {
    border-right: 2px solid #fff;
    border-left: 2px solid #fff;
  }
  .card {
    color: #fff;
    p {
      font-weight: bold;
      line-height: 1.9;
      font-size: 18px;
    }
    span {
      font-weight: bold;
      line-height: 1.9;
      font-size: 18px;
      color: #14365d;
      position: relative;
      &::before {
        position: absolute;
        content: "";
        left: 0px;
        bottom: -10px;
        height: 5px;
        width: 55px;
        background: #ffffff;
        padding: 4px;
        border-radius: 4px;
      }
    }
  }
}
</style>
