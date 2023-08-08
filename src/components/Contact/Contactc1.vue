<template>
  <div class="contactc1">
    <v-container>
      <h1 class="mt-16 mb-16">Contact Us Now</h1>
      <v-row>
        <form @submit.prevent class="ma-auto d-flex flex-column text-center">
          <div class="phone d-flex flex-column text-center">
            <label for="">PHONE</label>
            <input type="number" readonly placeholder="01098778859" />
          </div>
          <div class="email d-flex flex-column text-center">
            <label for="">EMAIL</label>
            <input
              type="number"
              readonly
              placeholder="abdokhalef29@gmail.com"
            />
          </div>
          <div class="social">
            <label>SOCIAL</label>
            <ul class="d-flex justify-center mt-8">
              <li>
                <a href="#">
                  <v-icon>mdi-facebook</v-icon>
                </a>
              </li>
              <li>
                <a href="#">
                  <v-icon>mdi-twitter</v-icon>
                </a>
              </li>
              <li>
                <a href="#">
                  <v-icon>mdi-instagram</v-icon>
                </a>
              </li>
            </ul>
          </div>
        </form>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "ContactC1",
};
</script>

<style lang="scss" scoped>
.contactc1 {
  background: #14365d;
  color: #fff;
  height: 92.2vh;
  form {
    gap: 50px;
    .phone,
    .email,
    .social {
      label {
        font-weight: bold;
        font-size: 24px;
        margin-bottom: 10px;
      }

      input {
        cursor: pointer;
        outline: none;
        border: 1px solid #fff;
        border-radius: 25px;
        font-size: 24px;
        width: 500px;
        &::placeholder {
          padding: 10px;
          width: 100%;
          color: #000;
          text-align: center;
          background: #fff;
        }
      }
    }
    .social {
      ul {
        gap: 50px;
        li {
          a {
            color: #fff;
          }
        }
      }
    }
  }
}
</style>
