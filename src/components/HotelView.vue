<template>
  <main class="hotel-view">
    <HotelView_gallery />
    <HotelView_overview />
    <HotelView_description />
    <HotelView_cta />
  </main>
</template>

<script>
import HotelView_gallery from "@/components/HotelView_gallery.vue";
import HotelView_overview from "@/components/HotelView_overview.vue";
import HotelView_description from "@/components/HotelView_description.vue";
import HotelView_cta from "@/components/HotelView_cta.vue";

export default {
  components: {
    HotelView_gallery,
    HotelView_overview,
    HotelView_description,
    HotelView_cta
  }
};
</script>

<style lang="scss" scoped>
.hotel-view {
  background-color: #fff;

  flex: 1;
}
</style>
