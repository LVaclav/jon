<template>
  <nav
    class="navbar fixed-top navbar-expand-lg navbar-dark bg-grey justify-content-center"
  >
    <a type="button" class="nav-link text-white shadow-none" @click="setAbout"
      >About</a
    >
    <a
      type="button"
      class="navbar-brand text-white shadow-none fw-bold px-4"
      @click="setHome"
      >Jons Photog</a
    >
    <a type="button" class="nav-link text-white shadow-none" @click="setBooking"
      >Booking</a
    >
  </nav>

  <div v-show="caroselState">
    <DemoCarosel></DemoCarosel>
  </div>

  <div v-show="aboutState">
    <AboutBlock></AboutBlock>
  </div>

  <div v-show="bookingState">
    <bookingBlock></bookingBlock>
  </div>
</template>

<script>
import DemoCarosel from "./components/DemoCarosel.vue";
import AboutBlock from "./components/AboutBlock.vue";
import bookingBlock from "./components/bookingBlock.vue";

export default {
  name: "app",
  components: {
    DemoCarosel,
    AboutBlock,
    bookingBlock,
  },
  data() {
    return {
      caroselState: true,
      aboutState: false,
      bookingState: false,
    };
  },
  methods: {
    setHome: function () {
      (this.aboutState = false),
        (this.caroselState = true),
        (this.bookingState = false);
    },
    setAbout: function () {
      (this.aboutState = true),
        (this.caroselState = false),
        (this.bookingState = false);
    },
    setBooking: function () {
      (this.aboutState = false),
        (this.caroselState = false),
        (this.bookingState = true);
    },
  },
};
</script>

<style>
#app {
  text-align: center;
}
</style>
