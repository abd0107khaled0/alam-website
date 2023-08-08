<template>
  <div>
    <v-form ref="form" class="mx-2" lazy-validation>
      <v-text-field :rules="inputRules" v-model="da"> </v-text-field>
      <v-btn class="purple darken-2 white--text mt-5" @click="submitForm">
        Register
      </v-btn>
    </v-form>
  </div>
</template>

<script>
export default {
  name: "RegisterV",
  data() {
    return {
      da: "",
      inputRules: [(v) => v.length >= 5 || "this is low"],
    };
  },
  methods: {
    submitForm() {
      if (this.$refs.form.validate()) {
        console.log("yes");
      }
    },
  },
};
</script>

<style></style>
