<template>
  <div class="homec2">
    <v-container>
      <h1 color="white" class="mb-16">Best Reviews</h1>
      <v-row>
        <v-col
          cols="12"
          lg="4"
          md="6"
          sm="12"
          xs="12"
          v-for="n in 7"
          :key="n.id"
        >
          <v-card class="pa-10 card" rounded="xl" style="background: #14365d">
            <v-card-title>
              <v-icon>mdi-account</v-icon>
            </v-card-title>
            <v-card-text>
              <p class="mt-10 mb-10">
                Rewiew will be written here Rewiew will be written here Rewiew
                will be written here Name
              </p>
              <span> Name </span>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "HomeC2",
};
</script>

<style lang="scss" scoped>
.homec2 {
  background: #fff;
  padding: 90px 0;
  h1 {
    color: #14365d;
  }
  .card {
    color: #fff !important;
    p {
      font-weight: bold;
      line-height: 1.9;
      font-size: 18px;
    }
    span {
      font-weight: bold;
      line-height: 1.9;
      font-size: 18px;
      color: #fff;
      position: relative;
      &::before {
        position: absolute;
        content: "";
        left: -15px;
        top: 0;
        height: 55px;
        width: 5px;
        background: #794cec;
        padding: 4px;
        border-radius: 4px;
      }
    }
  }
}
</style>
