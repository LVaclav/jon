<template>
  <div class="test-filter">
    <img
      src="../assets/photos/back.jpg"
      style="width: 100%; filter: brightness(70%)"
    />
  </div>

  <div class="py-5"></div>

  <!-- Bios -->
  <div class="row justify-content-center">
    <!-- first person -->
    <div class="col-3 page-content-wrap" style="text-align: center">
      <div style="text-align: left">
        <div class="row">
          <img
            class="col-4 img-fluid"
            src="../assets/photos/jon.png"
            alt="jon_pfp"
            style="height: 100%"
          />
          <div class="col-2"><h2>Jon Copson</h2></div>
        </div>

        <p>
          <span
            >Jon is a cool guy, gets shit done and can be your next best friend.
            HE does lots of stuff and things done</span
          >
        </p>
      </div>
    </div>
    <!-- second person  -->
    <div class="col-3 page-content-wrap" style="text-align: center">
      <div style="text-align: left">
        <div class="row">
          <img
            class="col-4 img-fluid"
            src="../assets/photos/jason.jpg"
            alt="jason_pfp"
            style="height: 100%"
          />
          <div class="col-2"><h2>Jason Baker</h2></div>
        </div>
        <p>
          <span>
            Jason is a cool guy, gets shit done and can be your next best
            friend. HE does lots of stuff and thing
          </span>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutPage",
};
</script>

<style>
#AboutPage {
  text-align: center;
}
</style>
