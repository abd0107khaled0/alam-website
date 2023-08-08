<template>
  <div class="nav">
    <homec />
    <homec-2 />
    <homec-3 />
  </div>
</template>

<script>
import Homec from "@/components/Home/Homec1.vue";
import Homec2 from "@/components/Home/Homec2.vue";
import Homec3 from "@/components/Home/Homec3.vue";
export default {
  components: { Homec, Homec2, Homec3 },
  name: "HomeV",
};
</script>

<style lang="scss" scoped>
div.nav {
  height: 100vh;
}
</style>
