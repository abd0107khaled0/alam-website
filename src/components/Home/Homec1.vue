<template>
  <div class="homec1">
    <v-container>
      <div class="content">
        <h4>
          Ayman <br />
          ALLAM
        </h4>
        <p>CEM<br />COURSES</p>
        <span> CHEMSTRY COURSES </span>
      </div>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "HomeC1",
  data() {
    return {
      firstname: "",
      lastname: "",
      nameRules: [
        (v) => !!v || "Name is required",
        (v) => (v && v.length <= 10) || "Name must be less than 10 characters",
      ],
    };
  },
  methods: {
    submitForm() {
      console.log(this.$refs.form);
      if (this.$refs.form.validate()) {
        console.log("yes");
      }
    },
  },
};
</script>

<style lang="scss" scoped>
.homec1 {
  padding: 50px 0;
  background: var(--main-color);
  background-image: url("../../../src/assets/img/bg.png");
  background-size: cover;
  height: 103.5vh;
  .content {
    transform: translateY(50%);
    margin: -100px auto;
    text-align: center;
    h4 {
      color: #fff;
      font-size: calc(10px + 1vw);
      font-weight: bold;
      line-height: 1.4;
      width: fit-content;
      margin: 0 auto;
    }
    p {
      color: #fff;
      font-weight: bold;
      font-size: calc(30px + 2vw);
      line-height: 1.3;
      margin: 24px 0;
    }
    span {
      color: #fff;
      font-size: calc(10px + 1.2vw);
      font-weight: bold;
      line-height: 1.4;
      position: relative;
      width: fit-content;
      margin: 0 auto;
    }
  }
}
</style>
