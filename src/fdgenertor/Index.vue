<template>
  <div>
    <img src="../assets/image/background.png" class="background" />
    <left-card></left-card>
  </div>
</template>

<script>
import LeftCard from "./components/LeftCard.vue";

export default {
  name: "Index",
  components: {
    LeftCard,
  },
};
</script>

<style lang="scss" scoped>
.background {
  width: 100%;
  position: absolute;
  z-index: -1;
}
</style>
