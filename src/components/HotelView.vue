<template>
  <main class="hotel-view">
    <HotelView_gallery />
    <HotelView_overview />
    <HotelView_description />
  </main>
</template>

<script>
import HotelView_gallery from "@/components/HotelView_gallery.vue";
import HotelView_overview from "@/components/HotelView_overview.vue";
import HotelView_description from "@/components/HotelView_description.vue";

export default {
  components: {
    HotelView_gallery,
    HotelView_overview,
    HotelView_description
  }
};
</script>

<style lang="scss" scoped>
.hotel-view {
  background-color: #fff;

  flex: 1;
}
</style>
