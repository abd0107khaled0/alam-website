<template>
  <div class="nav">
    <nav>
      <v-container>
        <v-row>
          <v-col lg="4" class="text-left">
            <h1 color="white" style="color: #fff">CEMcourses</h1>
          </v-col>
          <v-col lg="8" class="text-right">
            <ul class="d-flex justify-end">
              <li>
                <router-link to="/">HOME</router-link>
              </li>
              <li>
                <router-link to="/courses">Courses</router-link>
              </li>
              <li>
                <router-link to="/about">About Us</router-link>
              </li>
              <li>
                <router-link to="/contact">Contact Us</router-link>
              </li>
            </ul>
          </v-col>
        </v-row>
      </v-container>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.nav {
  // position: fixed;
  // width: 100%;
  background: #14365d;
  nav {
    ul {
      gap: 40px !important;
      margin-top: 9px;
      li {
        a {
          font-weight: bold;
          color: #fff;
          padding: 5px;
          transition: all 0.3s ease-in-out;
          &.router-link-exact-active {
            color: #ffffff;
            font-size: 18px;
            border-bottom: 3px solid #fff;
          }
        }
      }
    }
  }
}
</style>
