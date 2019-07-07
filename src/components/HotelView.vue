<template>
  <main class="hotel-view">
    <HotelView_gallery />
    <HotelView_overview />
  </main>
</template>

<script>
import HotelView_gallery from "@/components/HotelView_gallery.vue";
import HotelView_overview from "@/components/HotelView_overview.vue";
export default {
  components: {
    HotelView_gallery,
    HotelView_overview
  }
};
</script>

<style lang="scss" scoped>
.hotel-view {
  background-color: #fff;

  height: 80vh;

  flex: 1;
}
</style>
