<template>
  <div class="py-3"></div>

  <img src="../assets/photos/back.jpg" style="width: 100%" />

  <div class="py-5"></div>

  <!-- Bios -->
  <div class="row justify-content-center px-4">
    <!-- first person -->
    <div
      class="col-md-3 page-content-wrap"
      style="text-align: center"
      v-for="(bio, key) in bios"
      v-bind:key="key"
    >
      <div style="text-align: left">
        <div class="row">
          <img
            class="col-sm-4 img-fluid"
            :src="bio.src"
            :alt="bio.photoAlt"
            style="height: 100%"
          />
          <div class="col-sm-2">
            <h2>{{ bio.name }}</h2>
          </div>
        </div>

        <p class="text-muted">
          <span>{{ bio.paragraph }} </span>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutPage",
  data() {
    return {
      bios: [
        {
          name: "Jon Copson",
          src: "https://i.ibb.co/XF83jQP/jon-dc8d3077.png",
          photoAlt: "Jon Pfp",
          paragraph:
            "Jon Copson is our lead cinamatographer. With years of film expiernce and media oriented education, he brings a creative and cinamtic look to your event. He is passioante about his work and your needs.",
        },
        {
          name: "Jason Baker",
          src: "https://i.ibb.co/31mHmQt/jason-36f02c26.jpg",
          photoAlt: "Jason PFP",
          paragraph:
            "Jason baker is the backbone of your next production. A mind of planning, and years of industry expiernce make him the perfect guy to fuel your next cinematic adventure.",
        },
      ],
    };
  },
  mounted() {},
};
</script>

<style>
#AboutPage {
  text-align: center;
}
</style>
