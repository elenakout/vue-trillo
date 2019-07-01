<template>
  <div class="main-trillo">
    <div class="container">
      <Header />
      <div class="content">
        <sidebar />
        <hotel-view />
      </div>
    </div>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Sidebar from "@/components/Sidebar.vue";
import HotelView from "@/components/HotelView.vue";
export default {
  components: {
    Header,
    Sidebar,
    HotelView
  }
};
</script>

<style lang="scss"></style>
